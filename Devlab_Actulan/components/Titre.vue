<template>
    <div>
        <h4>{{ text }}</h4>
        <p><img src="../assets/img/Ligne.png" alt="LigneImage"></p>
    </div>
</template>

<script>
export default{
    
    props: ["text"]
}
</script>

<style scoped>
    *{
        float: left;
        width: max-content;
    }

h4  {
    margin-left: 50px;
    font-size: 50px;
  font-weight: 500;
   color: #6e66c8;
    }
    p{
        
        font-size: 22px;
        font-weight: 500;
        color: #6E66C8;
        display: inline;
        margin: 10px;
    }

    img{
        margin-top: 20px;
        margin-left: 30px;
       
    }

</style>