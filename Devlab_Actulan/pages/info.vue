<template>
    <div>
        <Header/>

        <section class="main">
            <br>
            <article class="titleh1">
            <h1>13ATable Lan</h1>
            </article>

            <section class="FirstPart" id="pad">
                <InfoLans/>
                <img src="../assets/img/carte.png">
            </section>

            <section class="SecondPart" id="pad">
                <Titre/>
                <p>L’association 13àtable.lan est une association à but non lucratif (loi 1901).<br><br>
                Notre objectif est d’organiser des LANs Party dans le Sud de la France de façon à redorer l’image du jeu vidéo en valorisant son aspect communautaire et social. 
                Trop souvent montré du doigt par les médias comme source d’exclusion et d’isolement nous tenons à démontrer à travers l’organisation de LANs que le jeu vidéo peut se vivre comme une passion, un sport  et donc procurer les même sensations.<br><br>
                Une victoire, l’esprit d’equipe, la strategie et la solidatrité autant de valeur que nous partageons avec n’importe quel passioné.<br><br>
                Une association réunie autour d’une passion commune : le jeu vidéo et l’informatique.<br><br>
                Notre association, 13 à table.</p>
            </section>

            <section class="ThirdPart" id="pad">
                <Titre/>
                <ul>
                    <li>Samedi 10 mars 2012 - #07LAN 13AT - WINTER GAMING EDITION 2011 à Martigues (13500) - 50 places</li>
                    <li>Samedi 29 octobre 2011 - #06LAN 13AT - AUTOMN GAMING EDITION 2011 à Martigues (13500) - 70 places</li>
                    <li>Samedi 19 février 2011 - #05LAN 13AT - WINTER GAMING EDITION 2011 à Martigues (13500) - 70 places</li>
                    <li>Samedi 4 décembre 2010 - #04LAN 13AT - TELETHON - Games4Life à Chateau neuf les martigues (13500) - 100 places</li>
                    <li>Samedi 23 octobre 2010 - #03LAN 13AT - AUTOMN GAMING EDITION 2010 à Martigues (13500) - 50 places</li>
                    <li>Samedi 17 avril 2010 - #02LAN 13AT - SPRING GAMING EDITION 2010 à Martigues (13500) - 100 places</li>
                    <li>Samedi 31 octobre 2009 - #01LAN 13AT - HALLOWEEN GAMING EDITION 2009 à Martigues (13500) - 50 places</li>
                </ul>
                <BoutonEvenement/>
            </section>

            <br><br>

        </section>

        <Footer/>
    </div>
</template>


<script>

    import Header from '../components/Header';
    import InfoLans from '../components/InfoLans';
    import Titre from '../components/Titre';
    import BoutonEvenement from '../components/BoutonEvenement';
    import Footer from '../components/Footer';

    export default{
        components:{
            Header,
            InfoLans,
            Titre,
            BoutonEvenement,
            Footer
        }
    }

</script>


<style scoped>

    .main{
        background: linear-gradient(#667EEA, #764BA2);
    }

    #pad{
        margin: 5% 5% 0 5%;
    }

    /* Pas touche */
    .main section{ 
        margin: 5% 0;
    }

    .titleh1{
        height: fit-content;
        background-color: #FFFFFF;
        text-align: center;
        margin-top: 3%;
    }

    .FirstPart{
        height: fit-content;
        display: flex;
    }

    .SecondPart{
        height: fit-content;
        border-radius: 13px;
        background-color: #FFFFFF;
        padding: 40px;
    }

    .ThirdPart{
        height: fit-content;
        border-radius: 13px;
        background-color: #FFFFFF;
        padding: 40px;
    }

    p{
        font-size: 25px;
        color: #6E66C8;
        padding: 140px 420px 0 90px;
    }

    ul{
        margin-top: 120px;
    }

    li{
        font-size: 25px;
        color: #6E66C8;
        padding: 20px;
        list-style: none;
    }

    button{
        margin-left: 78%;
        text-align: center;
    }

    img{
        width: 50%;
        height: 90%;
        margin: 6% 0 6% 3%;
    }

    h1{
        padding: 20px;
    }

    h4{
        color: #6E66C8;
    }

    @media screen and (max-width: 1122px){

        .FirstPart{
            display: block;
        }

        img{
            width: 100%;
            height: 100%;
            margin: 0;
            margin-top: 50px;
        }

        p{
            padding: 120px 200px 0 90px;
        }

        button{
            margin-left: 72%;
        }
    }

     @media screen and (max-width: 825px){
         p{
            padding: 120px 100px 0 70px;
         }

         button{
            display: none;
         }

         h1{
            padding: 5% 0 0 5%;
            font-size: 26px;
            font-weight: bold;
            text-align: initial;
         }

         .FirstPart{
             padding: 0 5%;
         }

         .SecondPart{
             background: linear-gradient(#667EEA, #6E64C6);
         }

         .ThirdPart{
             background: linear-gradient(#6E64C6, #764BA2);
         }

         .main{
             background: #FFFFFF;
         }

         p, li{
            font-size: 22px;
            color: #FFFFFF;
         }

         h4{
            color: #FFFFFF;
         }

         #pad{
            margin: 0;
            border-radius: 0;
         }
     }

</style>