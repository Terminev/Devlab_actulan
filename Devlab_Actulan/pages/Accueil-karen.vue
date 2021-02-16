<template>
  <div>
    <section>
      <img src="~/assets/img/mapactulan.png" alt="carte map">
      <img src="~/assets/img/mapactulanMobile.png" alt="carte map">
      <article>
        <h2>Nos<br>prochaines<br>lans</h2>
        <div>
          <p>voir les dates</p>
          <img src="~/assets/img/flechegauche.png" alt="flechegauche">
        </div>
      </article>
    </section>

    <section>
      <img src="~/assets/img/calendar.png" alt="calendrier">
      <div>
        <LanCalendrier date="15/01" titre="Nanatera" place="15 places" />
        <LanCalendrier date="15/01" titre="Nanatera" place="15 places" />
        <LanCalendrier date="15/01" titre="Nanatera" place="15 places" />
        <LanCalendrier date="15/01" titre="Nanatera" place="15 places" />
        <LanCalendrier date="15/01" titre="Nanatera" place="15 places" />
      </div>
    </section>

    <section>
      <div>
        <ul>
          <li>Créer associations et évènements avec la communauté Actu-Lan !</li>
          <li>Participer et s'inscrire auprès de diffèrentes associations et évènements !</li>
        </ul>
        <ul>
          <li>Commenter et discuter avec la communauté Actu-Lan !</li>
          <li>Partager des images de ces moments inoubliables dans la galerie d'images !</li>
        </ul>
      </div>
      <button>S'incrire</button>
    </section>
  </div>
</template>
<script>
  import LanCalendrier from '~/components/LanCalendrier.vue';

  export default {
    components: {
      LanCalendrier
    }
  }

</script>
<style scoped>
  *{
    box-sizing: border-box;
  }

  section:first-child img {
    position: relative;
    width: 100%;
  }

  section:first-child img+img {
    display: none;
  }

  section:first-child article {
    position: absolute;
    background-color: white;
    padding: 80px 250px 80px 105px;
    top: 280px;
    right: 0;
    border-radius: 13px 0 0 13px;
  }

  section:first-child h2 {
    font-size: 55px;
    font-weight: 500;
    text-transform: uppercase;
  }

  section:first-child article div {
    display: flex;
    margin-top: 50px;
    align-items: center;
  }

  section:first-child article div p {
    font-size: 35px;
    font-weight: 500;
    color: #6e66c8;
  }

  section:first-child article div img {
    width: 33px;
    height: 27.2px;
    margin-left: 50px;
  }

  section:nth-child(2){
    border-radius: 13px;
    border: solid 1px #707070;
    background-color: #ffffff;
    margin: 260px auto;
    width: 80%;
    display: flex;
    padding: 35px 90px;
  }

  section:nth-child(2) img{
    width: 600px;
  }

  section:nth-child(2) div{
    width: 100%;
    margin-left: 50px;
  }

  section:nth-child(2) div div{
    width: 100%;
    margin: 10px 0px;
  }

  section:last-child{

  }

  @media screen and (max-width: 1380px) {
    section:first-child article {
      padding: 50px 150px 50px 85px;
      top: 215px;
    }

    section:first-child h2 {
      font-size: 45px;
    }

    section:first-child article div p {
      font-size: 25px;
    }

    section:first-child article div img {
      width: 23px;
      height: 20px;
      margin-left: 30px;
    }

    section:nth-child(2){
      padding: 35px 30px;
    }
  }

  @media screen and (max-width: 900px) {
    section:first-child article {
      width: 100%;
      padding: 30px;
      border-radius: 35px 35px 0 0;
      box-shadow: 0 -3px 6px 0 rgba(0, 0, 0, 0.16);
      position: relative;
    }

    section:first-child img:first-child {
      display: none;
    }

    section:first-child img+img {
      display: block;
      width: 100%;
    }

    section:first-child h2 {
      font-size: 35px;
    }

    section:first-child article div {
      display: block;
      margin-top: 0;
    }

    section:first-child article div img {
      display: block;
      width: 47.2px;
      height: 55px;
      transform: rotate(90deg);
      margin: 70px auto 40px;
    }

    section:nth-child(2){
      border-radius: 0;
      border: none;
      width: 100%;
      display: block;
      padding: 0 0;
      margin-top: 80px;
    }

    section:nth-child(2) img{
      width: 600px;
    }

    section:nth-child(2) div{
      width: 100%;
      margin-left: 0px;
    }

    section:nth-child(2) div div{
      width: 80%;
      margin: 20px auto;
    }

    section:nth-child(2) img{
      width: 300px;
      display: block;
      margin : 0 auto;
    }

  }

@media screen and (max-width: 650px) {
    section:first-child article {
      top: 500px;
    }
}

@media screen and (max-width: 450px) {
    section:first-child article {
      top: 400px;
    }

    section:nth-child(2) div div{
      width: 90%;
    }
}
</style>
