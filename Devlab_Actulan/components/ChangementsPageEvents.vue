<template>
  <div class="changementdepage">
    <img src="../assets/img/white-arrow.png" id="flechegauche" />
    <p>{{ NumerosPage }}</p>
    <img src="../assets/img/white-arrow.png" />
  </div>
</template>
<script>
export default {
  name: "Changementdepages",
  props: ["NumerosPage"],
};
</script>

<style scoped>
.changementdepage {
  display: flex;
  margin-top: 100px;
  margin-left: 950px;
}

.changementdepage img {
  width: 2%;
}

p {
  padding: 0px 5px;
  color: white;
}
#flechegauche {
  transform: rotate(180deg);
}
</style>
