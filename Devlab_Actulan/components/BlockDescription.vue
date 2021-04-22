<template>
    <section>
        <div>
            <h2>Description</h2>
            <hr>
        </div>
        <p>Tournois disponible :</p>
        <ul>
            <li>CS:GO - place à 20€ - 16 équipes</li>
            <li>LOL - Place à 20€ - 16 équipes</li>
            <li>Rocket League - place à 10 € - 16 équipes</li>
        </ul>
        <p>N’hésitez pas à regarder le site pour d’autres informations : nantarena.net
            <br>
            Les lots et cashprizes à gagner seront annoncés ultérieurement.
        </p>
    </section>
</template>

<script>

</script>

<style scoped>
    section {
        padding: 5px 40px;
        background-color: white;
        border-radius: 13px;
        color: #6E66C8;
        width: 50%;
        padding-bottom: 80px;
    }

    div {
        display: flex;
    }

    div hr {
        border: 1.5px solid #6E66C8;
        height: 0px;
        margin: auto;
        width: 100%;
    }

    div h2 {
        margin-right: 40px;
        color:  #6E66C8;
        font-size: 50px;
        font-weight: 600;
        text-transform: uppercase;
    }

    ul {
        list-style: none;
        padding-left: unset;

    }

    ul li::before {
        content: '- ';
    }
</style>
