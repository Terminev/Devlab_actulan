<template>
    <button>
        <div>
            <p>Valider</p>
        </div>
        <div>
            <img src="img/checkedWhite.png" alt="checked">
        </div>
    </button>
</template>

<script>

</script>

<style scoped>
    button {
        width: 15%;
        height: 60px;
        border-radius: 47px;
        background-color: #6e66c8;
        border: none;
        border-style: none;
        display: flex;
        justify-content: space-around;
    }

    button p {
        font-size: 20px;
        font-weight: bold;
        letter-spacing: normal;
        color: #f4f3f3;
        padding-top: 20px;
        margin-left: 30px;
        text-transform: uppercase;
    }

    img {
        width: 25px;
    }

    div:last-child {
        padding-top: 15px;
    }


    @media screen and (max-width: 1300px) {
        button {
            width: 20%;

        }
    }

    @media screen and (max-width: 900px) {
        button {
            width: 30%;

        }
    }

    @media screen and (max-width: 650px) {
        button {
            width: 50%;

        }
    }

    @media screen and (max-width: 400px) {
        button {
            width: 80%;

        }
    }

    @media screen and (max-width: 200px) {
        button {
            width: 100%;

        }
    }
</style>