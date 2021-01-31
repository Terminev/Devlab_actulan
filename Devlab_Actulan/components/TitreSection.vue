<template>
   <p class="TitreSection">{{ titre }}</p>
</template>

<script>

export default{
    name: 'section',
    props: ["titre"]
}


</script>

<style scoped>
.TitreSection {
    background-color: #F4F3F3;
    width: 30%;
    padding: 3px;
    border: 1px solid black;
    border-radius: 15px;
    font-size: 30px;
    font-weight: bold;
    text-align: center;
    text-transform: uppercase;
    color: black;
}
</style>