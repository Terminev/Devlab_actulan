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
      <div class="LanCalendrier">
        <div>
          <span>
            <p>15/01</p>
            <h5>Nanatera</h5>
          </span>
          <p>15 places</p>
        </div>
         <div>
          <span>
            <p>15/01</p>
            <h5>Nanatera</h5>
          </span>
          <p>15 places</p>
        </div>
         <div>
          <span>
            <p>15/01</p>
            <h5>Nanatera</h5>
          </span>
          <p>15 places</p>
        </div>
         <div>
          <span>
            <p>15/01</p>
            <h5>Nanatera</h5>
          </span>
          <p>15 places</p>
        </div>
         <div>
          <span>
            <p>15/01</p>
            <h5>Nanatera</h5>
          </span>
          <p>15 places</p>
        </div>
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
  * {
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
    color: $violet;
  }

  section:first-child article div img {
    width: 33px;
    height: 27.2px;
    margin-left: 50px;
  }

  section:nth-child(2) {
    border-radius: 13px;
    border: solid 1px #707070;
    background-color: #ffffff;
    margin: 260px auto;
    width: 80%;
    display: flex;
    padding: 35px 90px;
  }

  section:nth-child(2) img {
    width: 600px;
  }

  /* Composant LanCalendrier */
  .LanCalendrier div {
    border: black solid 2px;
    display: flex;
    flex-wrap: nowrap;
    align-items: center;
    background-color: white;
    justify-content: space-between;
    padding: 5px 10px;
  }

  .LanCalendrier span {
    display: flex;
    align-items: center;
  }

  .LanCalendrier h5 {
    text-transform: uppercase;
    font-size: 22px;
    margin-left: 30%;
    font-weight: 500;
  }

  .LanCalendrier p:first-child {
    margin-left: 10px;
    background-color: $violet;
    padding: 18px 8px;
    color: white;
    font-size: 15px;
    font-weight: bold;
    border-radius: 50px;
  }

  .LanCalendrier p:last-child {
    font-size: 16px;
    margin: 20px;
    text-transform: uppercase;
  }

  @media screen and (max-width: 1024px) {
    .LanCalendrier p:first-child {
      font-size: 12px;
      padding: 16px 8px;
    }

    .LanCalendrier p:last-child {
      font-size: 14px;
    }

    .LanCalendrier h5 {
      font-size: 18px;
      margin-left: 15%;
    }
  }

  @media screen and (max-width: 901px) {
    .LanCalendrier div {
      box-shadow: 0 3px 6px 0 rgba(0, 0, 0, 0.16);
      background-color: #d8d5d5;
      border: none;
      height: 40px;
      border-radius: 13px;
    }

    .LanCalendrier p {
      margin: 0;
      font-size: 14px;
    }

    .LanCalendrier p:first-child {
      margin-left: -15px;
    }

    .LanCalendrier p:last-child {
      display: flex;
      justify-content: flex-end;
      margin: 10px;
    }
  }

  /* Fin composant */



  section:nth-child(2) .LanCalendrier {
    width: 100%;
    margin-left: 50px;
  }

  section:nth-child(2) .LanCalendrier div {
    width: 100%;
    margin: 10px 0px;
  }

  section:last-child {
    background-image: url(~assets/img/fondesportactulan.png);
    background-repeat: no-repeat;
    background-size: cover;
    width: 100%;
    padding: 200px 0 50px;
  }

  section:last-child div ul {
    font-size: 26px;
    display: flex;
    justify-content: center;
    font-weight: bold;
    color: #dfe3e8;
    margin-bottom: 150px;
  }

  section:last-child div ul li {
    font-size: 36px;
    font-weight: bold;
    color: #dfe3e8;
    width: 500px;
    margin: 0 65px;
  }

  button {
    width: 500px;
    height: 60px;
    border-radius: 20px;
    border: solid 1px #080000;
    background-color: #f4f3f3;
    font-size: 36px;
    font-weight: bold;
    text-align: center;
    color: #020202;
    text-transform: uppercase;
    margin: 0 auto;
    display: block;
  }

  button:hover {
    cursor: pointer;
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

    section:nth-child(2) {
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
      top: -50px;
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

    section:nth-child(2) {
      border-radius: 0;
      border: none;
      width: 100%;
      display: block;
      padding: 0 0;
      margin-top: 0px;
    }

    section:nth-child(2) img {
      width: 600px;
    }

    section:nth-child(2) .LanCalendrier {
      width: 100%;
      margin-left: 0px;
    }

    section:nth-child(2) .LanCalendrier div {
      width: 80%;
      margin: 20px auto;
    }

    section:nth-child(2) img {
      width: 300px;
      display: block;
      margin: 0 auto;
    }

    section:last-child {
      padding-top: 100px;
    }

    section:last-child div ul {
      display: block;
      margin: 0 10%;
    }

    section:last-child div ul li {
      font-size: 26px;
      width: 90%;
      margin: 50px 0;
    }

    button {
      margin-bottom: 100px;
      height: 40px;
      font-size: 24px;
      width: 80%;
    }

  }
  @media screen and (max-width: 450px) {
    section:nth-child(2) .LanCalendrier div {
      width: 90%;
    }

    section:last-child div ul li {
      font-size: 20px;
    }
  }
</style>
