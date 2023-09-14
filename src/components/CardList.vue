<script>
import axios from "axios";

export default {
  data() {
    return {
      title: "cards",
      cards: [],
    };
  },
  methods: {
    fetchCards() {
      axios
        .get("https://db.ygoprodeck.com/api/v7/cardinfo.php")
        .then((response) => {
          this.cards = response.data.data;
        });
    },
  },
  /*chiamata axios per lista carte(api)*/
  created() {
    this.fetchCards();
  },
};
</script>

<template>
  <!--contenitore ricerca cards-->
  <div class="search-container">
    <input type="text" />
  </div>
  <!--contenitore cards-->
  <div class="cards-container">
    <!--cards-->
    <div class="cards" v-for="card in cards" :key="card.id">
      <img :src="card.card_images[0].image_url" alt="" />
      <h3>{{ card.name }}</h3>
      <span>{{ card.archetype }}</span>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.search-container {
  margin: 1rem 10rem;
}
.cards-container {
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  justify-content: space-around;
  background-color: white;
  padding-top: 2rem;
  margin: 0 auto;
  width: 80%;
}
.cards {
  display: flex;
  flex-direction: column;
  text-align: center;
  background-color: hsl(33.46deg 64.46% 52.55%);
  margin: 1rem 1rem;
  width: calc((100% / 5) - 2rem);
  img {
    max-width: 100%;
  }
}
</style>
