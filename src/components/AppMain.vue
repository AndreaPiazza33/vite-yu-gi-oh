<script>
import CardList from "./CardList.vue";

export default {
  components: { CardList },
};
</script>

<template>
  <!--contenitore main-->
  <div class="main-container">
    <!--cards-->
    <CardList></CardList>
  </div>
</template>

<style lang="scss" scoped>
.main-container {
  width: 100%;
  background-color: hsl(33.46deg 64.46% 52.55%);
}
</style>
