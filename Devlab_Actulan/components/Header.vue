<template>
    <header>
        <div id="enteteHeader">
            <img src="img/logo.png" alt="Logo Actu-Lan">
            <form action="">
                <label for="rechercher">
                    <input type="search" placeholder="Rechercher..." name="rechercher">
                    <button type="submit">
                        <img src="img/loupe.png" alt="logo loupe">
                    </button>
                </label>
            </form>
            <div>
                <img src="img/user.png" alt="Icon de l'utilisateur">
                <img src="img/userMobile.png" alt="Icon de l'utilisateur violet">
                <img src="img/menu.png" alt="Icon menu burger">
                <a href="#" title="Connexion au compte utilisateur">connexion</a>
                <a href="#" title="Inscription à Actu-Lan">inscription</a>
            </div>
        </div>
        <nav class="nav">
            <a href="#" title="Calendrier Lan">Calendrier</a>
            <a href="#" title="Structure Lan">Structure</a>
            <a href="#" title="Galerie Lan">Galerie</a>
            <a href="#" title="Recherche Actu-Lan">Recherche</a>
            <a href="#" title="Archives Actu-Lan">Archives</a>
        </nav>
    </header>
</template>

<script>

</script>

<style scoped>
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