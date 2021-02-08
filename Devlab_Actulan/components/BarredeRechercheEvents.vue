<template>
  <form class="rechercher" action="">
    <label for="Rechercher">
      <input type="search" placeholder="Rechercher un organisme" />
      <button type="submit">
        <img
          class="loupe"
          src="../assets/img/loupe.png"
          alt="loupe"
          id="loupe"
        />
      </button>
    </label>
  </form>
</template>

<script>
export default {
  name: "BarreRechercheEvents",
};
</script>

<style scoped>
input {
  border-radius: 8px;
  padding: 5px;
  width: 300px;
}
button {
  background-color: white;
  border-radius: 9px;
  border: none;
  color: none;
}
.loupe {
  width: 60%;
}
.rechercher {
  position: relative;
}
.rechercher input[type="text"] {
  position: absolute;
  left: 0;
  width: 100%;
}
.rechercher button[type="submit"] {
  position: absolute;
  right: 4px;
  top: 6px;
}
</style>
