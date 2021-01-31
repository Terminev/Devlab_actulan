<template>
   <section id="body">
       <article id="map_bloc">
        <div id="bloc_gauche">
           <div  id="paragraphe">
            <p>
            NOS PROCHAINES LANS
           </p>
           </div>
           
           <div id="date">
            <span>
            voir les dates
           </span>
           <div>
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
               
               <aside id="date">
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
justify-content: center;
width: 876px;
height: 634px;
background-color: white;

position: absolute;
right: 0;

}

#bloc_gauche p{
width: 465px;
  height: 300px;
font-size: 75px;
  
  font-stretch: normal;
  font-style: normal;
  line-height: 1.33;
  letter-spacing: normal;
  text-align: left;
  color: #010005;

}
#date{
    width: 465px;
  height: 50px;
 display: flex;
 justify-content: space-between;

}
#date span{
  font-size: 55px;
  
  text-align: left;
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
#contour #date{
    width: 50%;
    height: 100%;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;

}

</style>