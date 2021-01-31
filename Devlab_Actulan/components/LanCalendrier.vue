<template>
    <div>
        <p>5/12</p>
        <p>nantarena 2.0</p>
        <p>192 places</p>
    </div>
</template>

<script>

</script>

<style scoped>
    div {
        
        border: black solid 3px;
        display: flex;
        flex-wrap: nowrap;
        align-items: center;
        background-color: white;
        width: 80%;
        height: 70px;
    }

    p {
        margin-left: 10%;
        text-transform: uppercase;
    }

    p:first-child {
        margin-left: 10px;
        background-color: #6e66c8;
        padding: 16px 8px;
        width: fit-content;
        color: white;
        font-size: 16px;
        font-weight: bold;
        border-radius: 50px;
    }

    p:last-child {
        display: flex;
        justify-content: flex-end;
        width: 50%;
        margin-left: 0;
    }
</style>