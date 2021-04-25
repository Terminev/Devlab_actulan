<template>
    <button>
        <p>octobre</p>
        <div class="upanddown">
            <div>
                <img src="../assets/img/upanddown.png" alt="">
            </div>
            <div>
                <img src="../assets/img/Dropdown.png" alt="">
            </div>
        </div>
    </button>
</template>

<script>

</script>

<style scoped>
    button {
        width: 100px;
        height: 30px;
        margin: 0 3px 0 2px;
        padding: 8px 15.1px 9px 17px;
        border-radius: 25px;
        background-color: #6E66C8;
        display: flex;
        justify-content: space-around;
    }

    button p {
        width: 49px;
        height: 11px;
        font-size: 10px;
        color: #f4f3f3;
        text-transform: uppercase;
    }

    .upanddown {
        display: flex;
        flex-direction: column;
        justify-content: center;
    }
</style>
