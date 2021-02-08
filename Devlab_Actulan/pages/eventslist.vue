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
      <ListeStructure
        Nom="Nom"
        Lieux="Lieux"
        Lans="Lans"
        Nom1="#DITIB2 FIFA 16 PS4"
        Lieux1="STRASBOURG"
        Lans1="1"
        Nom2="13ATable LAN"
        Lieux2="Martigues"
        Lans2="7"
      />
    </div>

    <div class="basdepageEvents">
      <ChangementsPageEvents NumerosPage="1/2" />
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
