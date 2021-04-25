<template>
   <div class="connexion-body">
      <div class="connexion-block">
        <TitreSection
        titre= "CONNEXION"/>
        <InputForm
        PlaceHolder= "PSEUDO"
        Name= "pseudo"/>
        <InputForm
        PlaceHolder= "MOT DE PASSE"
        Name= "password"/>
        <BoutonValider
        Text="Connexion"/>
        <p>OU</p>
        <Facebook />
        <NuxtLink id="inscription" to="/">S'INSCRIRE</NuxtLink>
        </div>

   </div>
</template>

<script>
import TitreSection from '~/components/TitreSection'
import InputForm from '~/components/InputForm'
import BoutonValider from '~/components/BoutonValider'
import Facebook from '~/components/Connexion/FacebookConnect'

export default {
  name: 'connexion',
  components: {
    TitreSection,
    InputForm,
    BoutonValider,
    Facebook,
  }
}

</script>

<style scoped>
.connexion-body {
  background-image: linear-gradient(161deg, #667eea 15%, #764ba2 70%);

}
.connexion-block{
  border-radius: 13px;

  width: 80%;
  margin: 100px auto;
  background-color: white;
  display: flex;
  align-items: center;
  flex-direction: column;


}
input{
  width: 50%;
  margin: 10px 0;
}
.TitreSection{
  margin-bottom: 70px;
  margin-top: -15px;
}
.BoutonValider{
  margin: 30px 0;

}
p{
  font-size: 41px;
  font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
  color: #6E66C8;
  font-weight:bold
}
.FacebookConnect{
  margin: 30px 0px;
}
#inscription{
  color: #4d4d4d;
  font-size: 26px;
  font-weight: bold;
  font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
  text-decoration: none;
  margin-bottom: 40px;
}

@media screen and (max-width: 640px) {
  .connexion-block{
    width: 95%;
  }
  .TitreSection{
    width: 95%;
  }
  input{
    width: 95%;
  }
  .BoutonValider{
    width: 95%;
  }
  .FacebookConnect{
    width: 95%;
  }

}

</style>
