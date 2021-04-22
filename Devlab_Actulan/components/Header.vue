<template>
    <header>
        <div id="enteteHeader">
            <nuxt-link to="/accueil"><img src="~/assets/img/logo.png" alt="Logo Actu-Lan"></nuxt-link>
            <form action="">
                <label for="rechercher">
                    <input type="search" placeholder="Rechercher..." name="rechercher">
                    <button type="submit">
                        <img src="~/assets/img/loupe.png" alt="logo loupe">
                    </button>
                </label>
            </form>
            <div>
                <img src="~/assets/img/user.png" alt="Icon de l'utilisateur">
                <img src="~/assets/img/userMobile.png" alt="Icon de l'utilisateur violet">
                <img src="~/assets/img/menu.png" alt="Icon menu burger">
                <nuxt-link to="/connexion">connexion</nuxt-link>
                <nuxt-link to="/inscription">inscription</nuxt-link>
            </div>
        </div>
        <nav class="nav">
            <nuxt-link to="/calendrier">Calendrier</nuxt-link>
            <nuxt-link to="/structure">Structure</nuxt-link>
            <nuxt-link to="/galerie">Galerie</nuxt-link>
            <nuxt-link to="/recherche">Recherche</nuxt-link>
            <nuxt-link to="/archives">Archives</nuxt-link>
        </nav>
    </header>
</template>

<script>

</script>

<style scoped>
    header{
        background-color: #ffffff;
    }
    
    a {
        font-size: 20px;
        text-decoration: none;
        color: black;
    }

    #enteteHeader {
        background-image: linear-gradient(to top, #667eea60, #667eea1e 70%);
        display: flex;
        padding: 10px 130px;
        justify-content: space-between;
        align-items: center;
    }

    #enteteHeader div {
        justify-content: center;
        display: flex;
    }

    #enteteHeader div a {
        padding: 0 12px;
    }

    #enteteHeader div img+a {
        border-right: 2px solid black;
    }

    #enteteHeader div img+img {
        display: none;
    }

    form {
        background-color: transparent;
        border: solid 1px black;
        height: 55px;
        width: 40%;
        display: flex;
        justify-content: space-between;
        border-radius: 27px;
        align-items: center;
    }

    form label {
        display: flex;
        height: 55px;
        justify-content: space-between;
        width: 90%;
        align-items: center;
    }

    form input {
        background-color: transparent;
        width: 90%;
        padding: 40px;
        border-style: none;
        outline: none;
    }

    form button {
        display: flex;
        align-items: center;
        border-style: none;
        height: 26px;
        width: 26px;
        background-color: transparent;
        cursor: pointer;
    }

    form input::placeholder {
        color: black;
        font-size: 15px;
        text-transform: uppercase;
    }

    nav {
        border-top: solid 2px #707070;
        border-bottom: solid 2px #707070;
        background-color: #667eea65;
        display: flex;
        justify-content: center;
        text-transform: uppercase;
        padding: 25px 0;
    }

    nav a {
        margin: 0 60px;
    }

    @media screen and (max-width:1200px) {
        #enteteHeader {
            padding: 10px;
        }

        nav a {
            margin: 0;
        }

        nav {
            justify-content: space-around;
        }
    }

    @media screen and (max-width:900px) {
        #enteteHeader {
            background-color: white;
            background-image: none;
            border-bottom: 2px solid #667EEA;
        }

        #enteteHeader div a {
            display: none;
        }

        form {
            display: none;
        }

        #enteteHeader div img+img {
            display: block;
            margin: 0 10px;
        }

        #enteteHeader div img:first-child {
            display: none;
        }

        nav {
            display: none;
        }
    }
</style>