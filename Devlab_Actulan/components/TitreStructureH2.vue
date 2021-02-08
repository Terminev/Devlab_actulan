<template>
  <div class="H2structure">
    <h2>{{ titre }}</h2>
  </div>
</template>

<script>
export default {
  name: "TitreStructureH2",
  props: ["titre"],
};
</script>

<style scoped>
h2 {
  font-size: 26px;
  font-weight: bold;
  color: #020202;
  margin: auto;
  margin-bottom: 100px;
  background: white;
  width: 400px;
  text-align: center;
  border-radius: 9px;
}
@media (max-width: 320px) {
  h2 {
    margin-bottom: 40px;
  }
}
</style>
