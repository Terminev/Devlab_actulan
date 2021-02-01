<template>
  <div class="eventslistbody">
    <div class="hautdepagestructure">
      <TitreStructureH2 />

      <div class="bouton">
        <BarredeRechercheEvents />
        <BoutonAjoutStructure />
      </div>
    </div>
    <TableauEvents />

    <div></div>
  </div>
</template>


<script>
export default {};
</script>


<style>
.eventslistbody {
  height: 150vh;
  background: linear-gradient(#667eea, #764ba2);
}
.bouton {
  display: flex;
  justify-content: space-around;
}
.hautdepagestructure {
  padding-top: 100px;
}
</style>