<template>
    <div id="etiquette">
        <p>5/12</p>
        <p>nantarena 2.0</p>
        <p>192 places</p>
    </div>
</template>

<script>

</script>

<style scoped>
    #etiquette {
        
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

    @media screen and (max-width: 901px) {
        #etiquette {
        box-shadow: 0 3px 6px 0 rgba(0, 0, 0, 0.16);
        background-color: #d8d5d5;
        border:none;
        display: flex;
        flex-wrap: nowrap;
        align-items: center;
       
        width: 80%;
        height: 40px;
        border-radius: 13px;
    }
    p {
        font-size: 14px;
        margin-left: 10%;
        text-transform: uppercase;
    }
     p:first-child {
        margin-left: -15px;
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
        padding-right: 20px;

    }
    }
</style>