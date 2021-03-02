<template>
   <p>{{ titre }}</p>
</template>

<script>

export default{
    name: 'section',
    props: ["titre"]
}


</script>

<style scoped>
p {
    background-color: #F4F3F3;
    width: 60%;
    padding: 6px 0px;
    border: 1px solid black;
    border-radius: 15px;
    font-size: 30px;
    font-weight: bold;
    text-align: center;
    text-transform: uppercase;
    color: black;
}

@media screen and (max-width:900px) {
  p{
      background-color: initial;
      border: none;
      padding: 0 0 0 100px;
      text-align: left;
      width: 100%;
  }
}
</style>
