<template>
    <button class="BoutonValider">

        <p>{{ Text }}</p>
<<<<<<< HEAD
        
        <div>
            
        </div>
=======

>>>>>>> Louis-Axel
        <div>
            <img src="../assets/img/checkedWhite.png" alt="checked">
        </div>
    </button>
</template>

<script>
export default {
    props: ['Text']
}

</script>

<style scoped>
    button {
        width: 30%;
        height: 60px;
        border-radius: 47px;
        background-color: #6E66C8;
        border: none;
        border-style: none;
        display: flex;
        justify-content: space-evenly;
        align-items: center;
    }

    button p {
        font-size: 20px;
        font-weight: bold;
        letter-spacing: normal;
        color: #f4f3f3;

        margin-left: 30px;
        align-items: center;
        justify-content: center;
        text-transform: uppercase;
    }

    img {
        width: 25px;
    }




    @media screen and (max-width: 1300px) {
        button {
            width: 30%;

        }
    }

    @media screen and (max-width: 900px) {
        button {
            width: 40%;

        }
    }

    @media screen and (max-width: 650px) {
        button {
            width: 60%;

        }
    }

    @media screen and (max-width: 400px) {
        button {
            width: 90%;

        }
    }

    @media screen and (max-width: 200px) {
        button {
            width: 100%;

        }
    }
</style>
