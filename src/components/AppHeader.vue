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
  <!--contenitore con img e titolo-->
  <div class="header-container">
    <span>img logo</span>
    <h2>Yu-Gi-Oh Api</h2>
  </div>
</template>

<style>
.header-container {
  display: flex;
  flex-direction: row;
  justify-content: left;
  align-items: center;
  gap: 1rem;
}
</style>
