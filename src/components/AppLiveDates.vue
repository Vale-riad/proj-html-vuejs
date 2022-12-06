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
          img: "https://upload.wikimedia.org/wikipedia/commons/thumb/5/59/Georgia_location_map.svg/1920px-Georgia_location_map.svg.png",
          description:
            "Lorem ipsum dolor, sit amet consectetur adipisicing elit. Itaque mollitia pariatur tempore expedita doloribus recusandae quas veniam dolores natus, vel perspiciatis ut numquam.",
          active: false,
        },
        {
          date: "31/10/2020",
          name: "OASIS FESTIVAL 2020",
          location: "MARRAKECH, MOROCCO",
          title: "Untold Stories",
          img: "https://upload.wikimedia.org/wikipedia/commons/thumb/5/59/Georgia_location_map.svg/1920px-Georgia_location_map.svg.png",
          description:
            "Lorem ipsum dolor, sit amet consectetur adipisicing elit. Itaque mollitia pariatur tempore expedita doloribus recusandae quas veniam dolores natus, vel perspiciatis ut numquam.",
          active: false,
        },
        {
          date: "07/11/2020",
          name: "MOGA FESTIVAL",
          location: "ESSAOURIA, MAROCCO",
          title: "Untold Stories",
          img: "https://upload.wikimedia.org/wikipedia/commons/thumb/5/59/Georgia_location_map.svg/1920px-Georgia_location_map.svg.png",
          description:
            "Lorem ipsum dolor, sit amet consectetur adipisicing elit. Itaque mollitia pariatur tempore expedita doloribus recusandae quas veniam dolores natus, vel perspiciatis ut numquam.",
          active: false,
        },
        {
          date: "10/12/2020",
          name: "ENVISION FESTIVAL",
          location: "UVITA, COSTA RICA",
          title: "Untold Stories",
          img: "https://upload.wikimedia.org/wikipedia/commons/thumb/5/59/Georgia_location_map.svg/1920px-Georgia_location_map.svg.png",
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
        <span v-if="event.active" class="plus">-</span>
        <span v-else class="plus">+</span>
        <span class="date">{{ event.date }}</span
        ><span class="name">{{ event.name }}</span
        ><span class="location">{{ event.location }} </span>
        <div class="map" v-show="event.active === true">
          <img :src="event.img" />
          <div class="info-event">
            <h6 class="py-3">{{ event.title }}</h6>
            <p class="info-p">{{ event.description }}</p>
            <button class="btn-book">BOOK NOW</button>
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

      img {
        width: 350px;
        height: auto;
      }
      .info-event {
        padding: 20px;
        padding-top: 10px;
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
