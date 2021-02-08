<template>
  <div class="eventslistbody">
    <div class="hautdepagestructure">
      <TitreStructureH2 titre="STRUCTURES" />

      <div class="bouton">
        <BarredeRechercheEvents />
        <BoutonAjoutStructure titre="AJOUTER UNE STRUCTURE" />
      </div>
    </div>

    <div id="ListeStructureEvents">
      <ListeStructure />
    </div>

    <div class="basdepageEvents">
      <ChangementsPageEvents />
    </div>
  </div>
</template>


<script>
import TitreStructureH2 from "../components/TitreStructureH2";
import BarredeRechercheEvents from "../components/BarredeRechercheEvents";
import BoutonAjoutStructure from "../components/BoutonAjoutStructure";
import ListeStructure from "../components/ListeStructure";
import ChangementsPageEvents from "../components/ChangementsPageEvents";

export default {
  components: {
    TitreStructureH2,
    BarredeRechercheEvents,
    BoutonAjoutStructure,
    ListeStructure,
    ChangementsPageEvents,
  },
};
</script>


<style>
.eventslistbody {
  height: 200vh;
  background: linear-gradient(#667eea, #764ba2);
}
.bouton {
  display: flex;
  justify-content: space-around;
}
.hautdepagestructure {
  padding-top: 100px;
}
.basdepageEvents {
  margin: auto;
}

#ListeStructureEvents {
  margin-top: 100px;
}
</style>
