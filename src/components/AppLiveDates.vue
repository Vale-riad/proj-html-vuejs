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
        },
        {
          date: "24/09/202",
          name: "GROOVEFEST",
          location: "DOMINICAL REPUBLIC",
        },
        {
          date: "31/10/2020",
          name: "OASIS FESTIVAL 2020",
          location: "MARRAKECH, MOROCCO",
        },
        {
          date: "07/11/2020",
          name: "MOGA FESTIVAL",
          location: "ESSAOURIA, MAROCCO",
        },
        {
          date: "10/12/2020",
          name: "ENVISION FESTIVAL",
          location: "UVITA, COSTA RICA",
        },
      ],
    };
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
      <li v-for="(event, index) in events">
        <span class="plus">+</span>
        <span class="date">{{ event.date }}</span
        ><span class="name">{{ event.name }}</span
        ><span class="location">{{ event.location }} </span>
      </li>
      <li></li>
    </ul>
  </section>
  <section class="ads text-center">
    <h4>VIEW ALL LIVE DATES</h4>
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
}
</style>
