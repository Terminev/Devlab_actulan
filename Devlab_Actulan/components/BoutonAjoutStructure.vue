<template>
  <button class="boutonstructure" type="button">
    <img
      src="../assets/img/fin.png"
      alt="
    plus"
      id="Plus"
    />
    {{ titre }}
  </button>
</template>

<script>
export default {
  name: "BoutonAjoutStructure",
  props: ["titre"],
};
</script>

<style scoped>
.boutonstructure {
  background-color: black;
  color: white;
  border-radius: 10px;
  display: flex;
  justify-content: center;
  padding-top: 8px;
  padding-bottom: 5px;
}

.boutonstructure img {
  width: 10%;
  padding: 0px 5px;
}

@media (max-width: 320px) {
  .boutonstructure {
    border-radius: 40px;
  }

  .boutonstructure img {
    width: 6%;
    padding: 0px 5px;
  }
}
</style>
