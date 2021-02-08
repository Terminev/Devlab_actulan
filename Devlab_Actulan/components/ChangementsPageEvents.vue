<template>
  <div class="changementdepage">
    <img src="../assets/img/fleche.png" id="flechegauche" />
    <p>1/2</p>
    <img src="../assets/img/fleche.png" />
  </div>
</template>
<script>
export default {};
</script>

<style scoped>
.changementdepage {
  display: flex;
  margin-top: 100px;
  margin-left: 950px;
}
p {
  padding: 0px 5px;
  color: white;
}
#flechegauche {
  transform: rotate(180deg);
}
</style>
