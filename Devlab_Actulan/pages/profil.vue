<template>
<div class="profil-body">
       
    <div class="block-profil">
        <TitreSection
        titre= "PROFIL"/>
        <div class="profil">
            <PhotoProfile/> 
                <div class="profil_txt">
                   <h3>Silvayn Loiliu</h3>
                    <p>Évènements inscrits </p>
                    <span>Nanterra 2.0</span>
                </div>
                <article class="profil_info">

                    <div>
                    <img src="../assets/img/user.png" alt="">
                    <p>SL_45</p>
                    </div>                   
                   <div>
                    <img src="../assets/img/indication.png" alt="">
                    <p>Dijon</p>
                   </div>                   
                    <div>
                    <img src="../assets/img/cake.png" alt="">
                    <p>21/09/19</p>
                    </div>
                    
                </article>
        </div>
    <BoutonEvenement
        Text="Ajouter en ami"/>
    </div>

    <div class="block-structure">
<Titre
 text="STRUCTURE"/>
    </div>
       
        <div class="block-evenement">
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

export default {
 TitreSection,
 TitreH2,
 PhotoProfile,
 BoutonEvenement,
 Titre,
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
    padding-top: 150px;
    padding-bottom: 150px;
}
.profil_txt h3{
font-size: 60px;
color: #6E66C8 ;
margin-bottom: 60px;
}
.profil_txt p{
font-size: 37px;
font-weight: 500;
color: #020202;
}
.profil_txt span{
 font-size: 21px;
font-weight: 500;
color: #020202;
}
.profil_info{
    display: flex;
    flex-direction: column;  
    justify-content: space-between;
    vertical-align: center; 
}
.profil_info div{
    display: flex;
   

}
.profil_info div img{
    
    width: 36px;
    height: 36px;
}
.profil_info div p{
    font-size: 30px;
  font-weight: bold;
  color: #020202;
  text-align: center;
  margin-left: 35px;
}
.profil_info div p:nth-child(2){
  text-transform: uppercase;
}

.block-structure{
  margin-top: 150px; 
    width: 70%;
    height: 400px;
    background-color: white;
}

.block-evenement{
  margin-top: 150px; 
    width: 70%;
    height: 400px;
    background-color: white;
}

@media screen and (max-width: 1025px) {
.profil_txt h3{
font-size: 50px;
color: #6E66C8 ;
margin-bottom: 60px;
}
.profil_txt p{
font-size: 30px;
font-weight: 500;
color: #020202;
}
.profil_txt span{
 font-size: 20px;
font-weight: 500;
color: #020202;
}



.profil_info div img{
    
    width: 30px;
    height: 30px;
}
.profil_info div p{
    font-size: 26px;
  font-weight: bold;
  color: #020202;
  text-align: center;
  margin-left: 30px;
}
.profil_info div p:nth-child(2){
  text-transform: uppercase;
}
}
@media screen and (max-width: 900px) {
.profil-body{
    background-color: white;
    display: flex;
    flex-direction: column;
    align-items: center;
}
.block-profil .TitreSection{
position:absolute;
top:150px
}
.block-profil{
 margin-top:0px;
   
    width: 100%;
     
}

.profil{ 
    width: 100%;
    height: 200px;
    display:flex;
    flex-wrap: wrap;
    padding-top: 100px;
    
}

.profil_txt h3{
font-size: 40px;
color: #6E66C8 ;
margin-bottom: 10px;
}

.profil_info{
    height: 150px;
    display: flex;
    flex-direction: column;  
    justify-content: space-around;
    vertical-align: center; 
}

.profil_info div p{
    font-size: 20px;
  font-weight: bold;
  color: #020202;
  text-align: center;
  margin-left: 20px;
}

@media screen and (max-width: 460px) {
.profil picture{
    padding-bottom: 60px;
}

.block-profil button{
    margin-top: 100px;
}




}

@media screen and (max-width: 400px) {
.profil picture{
    padding-bottom: 60px;
}
.profil_txt{
    padding-bottom: 60px;
}

.block-profil button{
    margin-top: 230px;
}
}







}
</style>