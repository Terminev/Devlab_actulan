<template>
    <article>
        <span></span>
        <img src="../assets/img/photo.png" alt="photo de profil">
        <img src="../assets/img/fleche.png" alt="flèche">
        <div>
            <h3>Rhom</h3>
            <p>J’aime beaucoup ta photo avec les joueurs…</p>
        </div>
    </article>
</template>

<script>
</script>

<style scoped>
    div {
        margin-left: 30px;
    }

    h3 {
        font-size: 30px;
        font-weight: 500;
        color: #6e66c8;
    }

    p {
        font-size: 18px;
        color: #4d4d4d;
        font-weight: bold;
        padding: 10px 0px 30px 20px;
    }

    article {
        padding: 10px 30px;
        display: flex;
        align-items: center;
        border-top: 3px dotted #6e66c8;
        border-bottom: 3px dotted #6e66c8;
    }

    img {
        width: 120px;
    }

    img+img {
        display: none;
    }

    span {
        width: 30px;
        height: 30px;
        background-color: #6e66c8;
        border-radius: 30px;
        box-shadow: 0 3px 6px 0 rgba(0, 0, 0, 0.16);
        margin-right: 20px;
    }

    @media screen and (max-width: 800px) {
        article {
            position: relative;
            padding: 10px;
            border-top: 0;
        }

        img {
            width: 80px;
        }

        img+img {
            display: block;
            width: 10px;
            position: absolute;
            right: 10px;
            top: 25px;
        }

        h3 {
            font-size: 20px;

        }

        div {
            margin-left: 10px;
        }

        p {
            font-size: 15px;
            color: #4d4d4d;
            font-weight: normal;
            padding: 10px 0px 0px;
        }

        span {
            width: 15px;
            height: 15px;
            border-radius: 15px;
            margin-right: 20px;
        }
    }
</style>