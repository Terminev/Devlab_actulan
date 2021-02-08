<template>
    <div class="TitreH3">
        <h3>{{Titre}}</h3>
        <hr>
    </div>
</template>

<script>
export default {
    props:['Titre']
}
</script>

<style  scoped>
    div {
        display: flex;
    }

    div hr {
        border: 1.5px solid #6E66C8;
        height: 0px;
        margin: auto;
        width: 70%;
        display: flex;
        justify-content: flex-end;

    }
    .TitreH3 h3 {
        padding-left: 40px;
        margin-right: 40px;
        color: #6E66C8;
        font-size: 50px;
        font-weight: 600;
        text-transform: uppercase;
    }
</style>