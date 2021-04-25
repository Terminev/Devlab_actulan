<template>
  <div class="profil-body">

    <div class="block-profil">
        <TitreSection
        titre= "PROFIL"/>
        <section class="profil">
            <div class="imgprofil">
                <PhotoProfile/>
            </div>

                <div class="profil_txt">
                   <h3>Silvayn Loiliu</h3>

                <div class="infomodif">
                    <label><img src="../assets/img/user.png" alt=""><input type="text" ></label>
                    <label><img src="../assets/img/indication.png" alt=""><input type="text" ></label>
                    <label><img src="../assets/img/cake.png" alt=""><input type="text" ></label>
                </div>
                </div>
        </section>
    <BoutonValider
    Text="Enregistrer les modifs"/>
    </div>



   <div id="block-structure">
<Titre
 text="STRUCTURE"/>
    </div>

        <div id="block-evenement">
<Titre
 text="ÉVÈNEMENTS"/>
    </div>




</div>







</template>








<script>
 import TitreSection from '~/components/TitreSection'
 import TitreH2 from '~/components/TitreH2'
 import PhotoProfile from '~/components/PhotoProfile'
 import BoutonEvenement from '~/components/BoutonEvenement'
 import Titre from '~/components/Titre'
 import BoutonValider from '~/components/BoutonValider'

export default {
 TitreSection,
 TitreH2,
 PhotoProfile,
 BoutonEvenement,
 Titre,
 BoutonValider,
}

</script>


<style scoped>
.profil-body{

    display: flex;
    flex-direction: column;
    align-items: center;
}
.block-profil{
    margin-top: 150px;

    width: 70%;
    height: 650px;
    background-color: white;
    display: flex;
    flex-direction: column;
    align-items: center;
}
.block-profil .TitreSection{
position:absolute;
top:300px
}




.profil{
    width: 100%;
    height: 200px;
    display:flex;
   justify-content: space-around;
    padding-top: 100px;
    padding-bottom: 150px;
}

.profil_txt{
    width: 60%;
    height: 100%;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
}
.profil_txt h3{

font-size: 60px;
color: #6E66C8 ;
}
.infomodif{
    display: flex;
    flex-wrap: wrap;
    width: 100%;

}
.infomodif label{
 margin-top: 50px;
padding-left: 20px;

}

.infomodif input{
width: 260px;
  height: 36px;
}

.infomodif label img{
    width: 40px;
    height: 40px;
    margin-right: 30px;


}


#block-structure{
  margin-top: 150px;
    width: 70%;
    height: 400px;
    background-color: white;
}

#block-evenement{
  margin-top: 150px;
    width: 70%;
    height: 400px;
    background-color: white;
}

@media screen and (max-width: 900px) {
  .profil-body{
      background-color: white;
      display: flex;
      flex-direction: column;
      align-items: center;
  }


  .block-profil{
 width: 100%;


}

  .block-profil .TitreSection{
margin: auto;
top:150px
}
.profil{
  display: flex;
  flex-direction: column;
  height: 70%;
  padding-top: 50px;
  padding-bottom: 90px;

}
.imgprofil {
  width:auto;
  display: flex;
margin: auto;
}
.profil_txt {
 display: flex;
margin: auto;
width: 60%;
}

.profil_txt h3{
  margin: auto;
font-size: 50px;
}

.infomodif label{
 margin-top: 40px;
padding-left: 20px;
width: 100%;

}

.infomodif input{
width: 80%;
  height: 26px;
}

.infomodif label img{
    width: 30px;
    height: 30px;
    margin-right: 20px;
}
}


@media screen and (max-width: 483px){
.profil_txt{
  width: 70%;
}
.profil_txt h3{
font-size: 40px;
}
.infomodif input{
width: 78%;
}

}

@media screen and (max-width: 425px){
.profil_txt{
  width: 90%;
}

.profil_txt {
 display: flex;
margin: auto;
width: 100%;
}

.infomodif input{

  height: 20px;
}

.infomodif label img{
    width: 26px;
    height: 26px;



}



}


</style>
