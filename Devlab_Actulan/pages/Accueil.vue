<template>
   <section id="body">
       <article id="map_bloc">
        <div id="bloc_gauche">
           <div  id="paragraphe">
            <p>
           nos prochaines lans
           </p>
           </div>
           
           <div id="date">
            <span>
            voir les dates
           </span>
           <div id="fleche">
            <img src="~/assets/img/flechegauche.png" alt="flechegauche">
           </div>
           
           </div>
           
       </div>
       </article>
       <article id="calendar_date">
           <div id="contour">
               <div id="calendar">
                <img src="~/assets/img/calendar.png" alt="flechegauche">
               </div>
               
               <aside id="composantdate">
                   <lan-calendrier>
                   </lan-calendrier>
                   <lan-calendrier>
                   </lan-calendrier>
                   <lan-calendrier>
                   </lan-calendrier>
                   <lan-calendrier>
                   </lan-calendrier>
                    <lan-calendrier>
                   </lan-calendrier>
                   
               </aside>
           </div>
       </article>
       <article id="esport">
         <div id="txt_btn">
           <div id="txt">
           <ul>
             <li>Créer associations et évènements avec la communauté Actu-Lan !</li>
             <li>Participer et s'inscrire auprès de diffèrentes associations et évènements !</li>
             
           </ul>
           <ul>
             <li>Commenter et discuter avec la communauté Actu-Lan !</li>
             <li>Partager des images de ces moments inoubliables dans la galerie d'images !</li>
           </ul>
           </div>
           
            <div id="btn">
            <button>S'incrire</button>
            </div>
           
         </div>
       </article>
       
   </section>
  
</template>


<script>

import LanCalendrier from '../components/LanCalendrier.vue'



export default {
    
    

    components:{
        LanCalendrier
    }
}
</script>


<style scoped>

#body{
background: linear-gradient(#667EEA, #754DA4, #764BA2 );
}
#map_bloc{
    height: 850px;
    display: flex;
    align-items: center;
    background-image: url(~assets/img/mapactulanv2.png);
    background-repeat: no-repeat;
    background-position-x: -500px;
}
#bloc_gauche{
display: flex;
flex-direction: column;
align-items: center;
justify-content: space-evenly;
width: 45%;
height: 600px;
background-color: white;

position: absolute;
right: 0;

}
#bloc_gauche #paragraphe{
  width: 55%;
}

#bloc_gauche p{
text-transform: uppercase;
 font-size: 4em;
color: #010005;
}
#date{
 width: 55%;
 display: flex;
 justify-content: space-between;

}
#date span{
  font-size: 3.5em;
  color: #6e66c8;
}

#date img{
  padding-top: 15px;
}

#calendar_date{
    padding-top: 270px;
    display: flex;
    justify-content: center;
    
  
}
#contour{
    width: 80%;
  height: 700px;
  border-radius: 13px;
  border: solid 1px #707070;
  background-color: #ffffff;
  display: flex;
  

}
#contour #calendar{
    width: 50%;
    height: 80%;
  display: flex;
  justify-content: center;
  align-items: center;

}
#contour #composantdate{
    width: 50%;
    height: 100%;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: space-evenly;

}
#esport{
  padding-bottom: 260px;
  margin-top: 260px;
  width: 100%;
  height: 1000px;
  background-image: url(~assets/img/fondesportactulan.png);
  background-repeat: no-repeat;
  background-position-x: -120px;
  display: flex;
  justify-content: center;
  align-items: center;

}
#txt_btn{
  display: flex;
  flex-direction: column;
  justify-content: space-around;
  align-items: center;
  width: 70%;
  height: 80%;
}
#txt{
  height: 65%;
  display: flex;
  justify-content: space-between;
padding-left: 100px;

}
#txt ul{
  display: flex;
  flex-direction: column;
  justify-content: space-between;

}
#txt li{
width: 85%;

font-size: 36px;
font-weight: bold;
text-align: left;
color: #dfe3e8;
}
#txt li::marker{

/*font-size: 70px;*/
color: #dfe3e8;
}
#btn{
  width: 45%;
}

#btn button{
  width: 100%;
  height: 60px;
  border-radius: 20px;
  border: solid 1px #080000;
  background-color: #f4f3f3;
  font-size: 36px;
  font-weight: bold;
  text-align: center;
  color: #020202;
  text-transform: uppercase;
}

@media screen and (max-width: 1129px) {
  #bloc_gauche #paragraphe{
  width: 55%;
}
#bloc_gauche #paragraphe p{
  font-size: 3em;
}
#date span{
  font-size: 3em;
  
}
#txt{
  width: 100%;
}
#txt ul{
  display: flex;
  flex-direction: column;
  justify-content: space-around;

}
#txt li{
width: 80%;

font-size: 28px;

}
}

@media screen and (max-width: 901px) {
#map_bloc{
    height: 800px;
    display: flex;
    justify-content: flex-end;
    background-image: url(~assets/img/mapactulanv2.png);
    background-repeat: no-repeat;
    background-position-x: -900px;
    background-position-y: -100px;
}
#bloc_gauche{
  display: initial;
  top: 350px;
  justify-content: initial;
  border-radius: 25px 25px 0% 0%;
  width: 100%;
  height: 560px;
  
}
#bloc_gauche #paragraphe{
  padding-top: 20px;
  width: 60%;
  padding-left: 30px;
}
#bloc_gauche #paragraphe p{
  font-size: 60px;
}
#date{
 width: 100%;
 display: flex;
 flex-direction: column;

}
#date span{
padding-left: 30px;

}
#date img{
  padding-left: 300px;
  display: flex;
  margin: auto;
 transform: rotate(90deg);
 
}

#calendar_date{
    padding-top:0px;
    display: flex;
    justify-content: center; 
}

#contour{
    width: 100%;
    height: 800px;
    border-radius: 0px;
    border: none;
    background-color: #ffffff;
    display: flex;
    flex-direction: column;
    align-items: center;
}
#contour #calendar{
    width: 50%;
    height: 80%;
  display: flex;
}
#contour #composantdate{
    width: 80%;
    height: 100%;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: space-evenly;

}
#esport{
  height: auto;
  padding-bottom: 0px;
  margin-top: 0px;
  

}
#txt_btn{
  width: 100%;
}
#txt{
 padding-left: 0;
  padding-bottom: 60px;
  width: 80%;
  height: 100%;
    display: flex;
    flex-direction: column;
    justify-content: space-evenly;
}
#txt ul{
  display: flex;
  align-items: center;
}
#txt li{
  padding-top: 60px;
  font-size: 30px;
}

#btn{
  width: 70%;
  padding-bottom: 30px;
}
}

@media screen and (max-width: 425px) {
  #bloc_gauche #paragraphe{
  width: 55%;
}
#bloc_gauche #paragraphe p{
  font-size: 2.4em;
}
#date span{
  font-size: 2.5em;
  
}

#txt li{
font-size: 24px;
width: 90%;

}
#btn button{
  height: 40px;
  font-size: 24px;
  
}
}


</style>