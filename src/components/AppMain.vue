<script>
export default {
  data() {
    return {
      title: "",
    };
  },
};
</script>

<template>
  <!--contenitore main-->
  <div class="main-container">
    <!--contenitore ricerca cards-->
    <div></div>
    <!--contenitore cards-->
    <div class="cards-container">
      <!--cards-->
      <div class="cards">
        <span>img card</span>
        <h3>nome card</h3>
        <span>tipo card</span>
      </div>
      <div class="cards">
        <span>img card</span>
        <h3>nome card</h3>
        <span>tipo card</span>
      </div>
      <div class="cards">
        <span>img card</span>
        <h3>nome card</h3>
        <span>tipo card</span>
      </div>
      <div class="cards">
        <span>img card</span>
        <h3>nome card</h3>
        <span>tipo card</span>
      </div>
      <div class="cards">
        <span>img card</span>
        <h3>nome card</h3>
        <span>tipo card</span>
      </div>
      <div class="cards">
        <span>img card</span>
        <h3>nome card</h3>
        <span>tipo card</span>
      </div>
      <div class="cards">
        <span>img card</span>
        <h3>nome card</h3>
        <span>tipo card</span>
      </div>
      <div class="cards">
        <span>img card</span>
        <h3>nome card</h3>
        <span>tipo card</span>
      </div>
      <div class="cards">
        <span>img card</span>
        <h3>nome card</h3>
        <span>tipo card</span>
      </div>
      <div class="cards">
        <span>img card</span>
        <h3>nome card</h3>
        <span>tipo card</span>
      </div>
      <div class="cards">
        <span>img card</span>
        <h3>nome card</h3>
        <span>tipo card</span>
      </div>
      <div class="cards">
        <span>img card</span>
        <h3>nome card</h3>
        <span>tipo card</span>
      </div>
      <div class="cards">
        <span>img card</span>
        <h3>nome card</h3>
        <span>tipo card</span>
      </div>
      <div class="cards">
        <span>img card</span>
        <h3>nome card</h3>
        <span>tipo card</span>
      </div>
      <div class="cards">
        <span>img card</span>
        <h3>nome card</h3>
        <span>tipo card</span>
      </div>
    </div>
  </div>
</template>

<style>
.main-container {
  display: flex;
  flex-direction: row;
  justify-content: center;
  background-color: hsl(33.46deg 64.46% 52.55%);
  height: 100vh;
}
.cards-container {
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  justify-content: space-around;
  background-color: white;
  padding-top: 2rem;
  width: 80%;
}
.cards {
  display: flex;
  flex-direction: column;
  text-align: center;
  background-color: hsl(33.46deg 64.46% 52.55%);
  margin: 1rem 1rem;
  width: calc((100% / 5) - 2rem);
  max-height: calc(100% / 3);
}
</style>
