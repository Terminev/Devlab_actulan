<template>
    <button class="FacebookConnect">
        <svg xmlns="http://www.w3.org/2000/svg" width="21.831" height="40.761" viewBox="0 0 21.831 40.761">
            <path id="Icon_awesome-facebook-f" data-name="Icon awesome-facebook-f" d="M22.01,22.928l1.132-7.377H16.064V10.764c0-2.018.989-3.985,4.159-3.985H23.44V.5A39.241,39.241,0,0,0,17.728,0C11.9,0,8.089,3.533,8.089,9.929v5.622H1.609v7.377h6.48V40.761h7.975V22.928Z" transform="translate(-1.609)" fill="#fdf5f5"/>
        </svg>

        
            <p>Se connecter avec FaceBook</p>
    
    </button>
</template>

<script>
export default {
    props: ['Text']
}

</script>

<style scoped>
    button {
        width: 500px;
        height: 60px;
        border-radius: 47px;
        background-color: #4553BA;
        border: none;
        border-style: none;
        display: flex;
        justify-content: space-around;
        align-items: center;

    }

    button p {
        font-size: 20px;
        font-weight: bold;
        letter-spacing: normal;
        color: #f4f3f3;
        padding-top: 5px;
        margin-left: 30px;
        align-items: center;
        text-transform: uppercase;
    }

    svg {
        width: 25px;
        
    }

    div {
        padding-top: 15px;
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