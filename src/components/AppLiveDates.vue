<script>
export default {
  name: "AppLiveDates",
  data() {
    return {
      events: [
        {
          date: "17/08/2020",
          name: "GEM FESTIVAL 2020",
          location: "ANAKALIA, GEORGIA",
          title: "Untold Stories",
          img: "https://upload.wikimedia.org/wikipedia/commons/thumb/5/59/Georgia_location_map.svg/1920px-Georgia_location_map.svg.png",
          description:
            "Lorem ipsum dolor, sit amet consectetur adipisicing elit. Itaque mollitia pariatur tempore expedita doloribus recusandae quas veniam dolores natus, vel perspiciatis ut numquam.",
          active: false,
        },
        {
          date: "24/09/202",
          name: "GROOVEFEST",
          location: "DOMINICAL REPUBLIC",
          title: "Untold Stories",
          img: "https://www.google.com/maps/vt/data=bDCVItW000GWwiKt3sG2mUzo7XLyWTBr1PS1G56ivIfhBO3OrypVyQduJscZyJEnz-UPBIvb4lS6xhSY1UlKO9JEfkKcmC-xP2m7EzOqGJZSmOedoA_eBeP_KjoWpNN578O6tLceCAZh9VTk3-dwhFm1j4mn7A0zeRbvr8XLpNTm2uRIDUZPm4ysB2a_CEpOE2NXdW60lQU5-jL80aG-fXkhfcN1Z4N42xkLALv7onwm7GlV0qBUjkokOuPc",
          description:
            "Lorem ipsum dolor, sit amet consectetur adipisicing elit. Itaque mollitia pariatur tempore expedita doloribus recusandae quas veniam dolores natus, vel perspiciatis ut numquam.",
          active: false,
        },
        {
          date: "31/10/2020",
          name: "OASIS FESTIVAL 2020",
          location: "MARRAKECH, MOROCCO",
          title: "Untold Stories",
          img: "https://www.google.com/maps/vt/data=4BkqIbRW42jnAUIzfo4lqfdQZfOUPDsvjl_z-KQJusqAeWLFAX6L6ZyKWnhyGkvpDjlrKvj_Wgp_H-eU-ySXa-6dDWwPkqEMTsdzKSJczJa9216erJIuBCwotXaBec4v-gc4OJxIjvmzXxcrgxevaOM5j0iUjG3ZqcCGCt_zay5yeBB18mpoPrFwrapcq1yeIwS0nmVDmQUHZdQqoArgpYx3D7Y5vaDpuyb-pknHbGdL3s6Q_mq_JJ_1-6I",
          description:
            "Lorem ipsum dolor, sit amet consectetur adipisicing elit. Itaque mollitia pariatur tempore expedita doloribus recusandae quas veniam dolores natus, vel perspiciatis ut numquam.",
          active: false,
        },
        {
          date: "07/11/2020",
          name: "MOGA FESTIVAL",
          location: "ESSAOURIA, MAROCCO",
          title: "Untold Stories",
          img: "https://www.google.com/maps/vt/data=SbGpsmF1i-9FTlsP8-aW-bbsiM-ie06BAbFNnuCywrDy5oq-Z0vFrzgsyOTLb-neKY1lD-2UkICyzCGaTy-wPr_aPcxhW6NvfxiIeN_Jiovb3IEPUykzjNqJ7POsZ6C6vPcRkZtxuJpJ9C1PcAep5-_FbfYvgldMwjWYuyZ2vr2UO3CgCLlpPxn45nvfNgaOoBSLAGi1LyDT9ZTnbpvUbuiPG6Vt2O9e3tk9JdLL8U5ibcGsTvRlWsuMuGM",
          description:
            "Lorem ipsum dolor, sit amet consectetur adipisicing elit. Itaque mollitia pariatur tempore expedita doloribus recusandae quas veniam dolores natus, vel perspiciatis ut numquam.",
          active: false,
        },
        {
          date: "10/12/2020",
          name: "ENVISION FESTIVAL",
          location: "UVITA, COSTA RICA",
          title: "Untold Stories",
          img: "https://www.google.com/maps/vt/data=XoK3WWwSqm_vA5sw9DmAzTW11wmuUDfxoqNz8Eh7ytVuw8xORGarSZ4dnmQiqkkD6BV4w6jonp70QBmzD_zS_PuhiCIoIq-FBA7MZrA6S6V7DCTlih-1ACwoBVA9EjYBDuJ-2JrXfV2LRYghpuKkr-UN1bgrhCcpqeKPyoSOon1tjWTAmU4SulOMTib2JGO-N6bZ3noTCU0tVLxRUkxs_Ai9WLy0tnMl-75L9k_biGc8IZ_ZL3hHjeRpzDVo",
          description:
            "Lorem ipsum dolor, sit amet consectetur adipisicing elit. Itaque mollitia pariatur tempore expedita doloribus recusandae quas veniam dolores natus, vel perspiciatis ut numquam.",
          active: false,
        },
      ],
    };
  },
  methods: {
    chooseEvent(index) {
      this.events[index].active = !this.events[index].active;
    },
  },
};
</script>

<template>
  <section class="live-dates">
    <div class="container text-center">
      <h2>Live Dates</h2>
      <hr class="ms-hr" />
      <span class="paragrafo">
        Lorem ipsum dolor, sit amet consectetur adipisicing elit. Itaque
        mollitia pariatur tempore expedita doloribus<br />
        suscipit nihil hic enim omnis consectetur iusto,<br />
        recusandae quas veniam dolores natus, vel perspiciatis ut numquam.
      </span>
    </div>

    <ul class="dates mt-5">
      <li v-for="(event, index) in events" @click="chooseEvent(index)">
        <span v-if="event.active" class="minus">-</span>
        <span v-else class="plus">+</span>
        <span class="date">{{ event.date }}</span
        ><span class="name">{{ event.name }}</span
        ><span class="location">{{ event.location }} </span>
        <div class="map" v-show="event.active === true">
          <div class="map-img">
            <img :src="event.img" />
          </div>
          <div class="info-event">
            <h6 class="py-3">{{ event.title }}</h6>
            <p class="info-p">{{ event.description }}</p>
            <button class="btn-book mt-2">BOOK NOW</button>
          </div>
        </div>
      </li>
      <li></li>
    </ul>
  </section>
  <section class="ads text-center">
    <div class="view">
      <h4>VIEW ALL LIVE DATES</h4>
    </div>
  </section>
</template>

<style lang="scss" scoped>
.live-dates {
  background-color: #252a33;
  padding: 50px;
  color: white;
  padding-bottom: 100px;

  .ms-hr {
    width: 144px;
    color: lightgray;
    margin-left: 584px;
  }
  .paragrafo {
    color: lightgray;
  }
  .paragrafo {
    font-size: 13px;
  }
  .dates {
    margin: auto;
  }
  ul {
    list-style: none;
    width: 70%;
    margin-left: 200px;
    margin-bottom: 50px;
  }
  li:not(:last-child) {
    color: #ec4958;
    background-color: #323844;
    margin: 5px;
    padding: 10px;

    .map {
      color: white;
      display: flex;
      padding: 20px;
      .map-img {
        padding: 10px;
      }

      img {
        width: 350px;
        height: auto;
      }
      .info-event {
        padding-left: 25px;
      }
      .info-p {
        color: #7d7b8d;
      }
      .btn-book {
        background-color: #ec4958;
        color: white;
        padding: 5px 15px 5px 15px;
        border: none;
      }
    }
  }
  .minus {
    background-color: #ec4958;
    padding: 1px 5px;
    color: white;
  }
  .plus {
    color: white;
    padding: 20px;
  }
  .date {
    padding: 5px;
  }
  .name {
    padding: 5px;
  }
  .location {
    padding: 5px;
  }
  span {
    font-size: 12px;
  }
}
.ads {
  background-color: #ec4958;
  height: 100px;
  h4 {
    color: white;
    padding: 30px;
  }
  h4 {
    font-size: 16px;
    line-height: 45px;
  }
  .view:hover h4 {
    background-color: white;
    color: black;
  }
}
</style>
