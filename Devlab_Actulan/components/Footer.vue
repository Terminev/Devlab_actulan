<template>
    <footer>
        <img src="img/logoBlanc.png" alt="Logo Actulan" />
        <p>Retrouvez nous sur les differents réseaux sociaux</p>
        <a href="" title="Facebook"><img src="img/facebook.png" alt="Logo Facebook" /></a>
        <a href="" title="Twitter"><img src="img/twitter.png" alt="Logo Twitter" /></a>
        <div>
            <a href="#" title="Calendrier lan">Calendrier</a>
            <a href="#" title="Cgu">Cgu</a>
            <a href="#" title="Structures lan">Structures</a>
            <a href="#" title="Communauté d'Actu-Lan">Communauté</a>
            <a href="#" title="Page Recherche d'information">Recherche</a>
            <a href="#" title="Annexes">Annexes</a>
            <a href="#" title="Formulaire de connexion">Connexion</a>
            <a href="#" title="Formulaire de contact">Contact</a>
        </div>
    </footer>
</template>

<script>

</script>

<style scoped>
    a,
    p {
        font-size: 20px;
        text-decoration: none;
        color: #c4f0fd;
    }

    footer {
        text-align: center;
        background-color: #4d4d4d;
        padding-bottom: 40px;
    }

    footer img {
        width: 450px;
    }

    footer a img {
        width: 65px;
        margin: 0 10px;
    }

    footer p {
        margin: 65px 0 35px;
        text-transform: uppercase;
        font-size: 30px;
        font-weight: bold;
    }

    footer div {
        display: flex;
        margin: 60px 0 0;
        justify-content: center;
    }

    footer div a {
        font-size: 20px;
        text-transform: uppercase;
        margin: 0 20px;
    }

    @media screen and (max-width: 1130px) {
        footer div {
            justify-content: space-around;
            flex-wrap: wrap;
        }

        footer div a {
            font-size: 20px;
            text-transform: uppercase;
            margin: 10px 10px 0;
        }
    }

    @media screen and (max-width: 600px) {
        footer div a {
            font-size: 15px;
        }

        footer img {
            width: 300px;
        }

        footer a img {
            width: 55px;
            margin: 0 10px;
        }

        footer p {
            margin: 45px 0 35px;
            font-size: 20px;
        }

        footer div {
            margin-top: 30px;
        }

        footer div a {
            font-size: 12px;
        }
    }
</style>