<template>
    <section>
        <div>
            <input type="search" placeholder="recherche...">
        </div>
        <ul>
            <li>Calendrier</li><hr>
            <li>Structure</li><hr>
            <li>Communauté</li><hr>
            <li>Recherche</li><hr>
            <li>Archives</li><hr>
        </ul>
        <div class="close">
            <span>X</span>
        </div>
    </section>
</template>

<script>
    
</script>

<style scoped>
hr {
    background-color: #667EEA;
    height: 2px;
    border: none;
}

section {
    width: 100%;
    height: 100vh;
}

div{
    background-color: #667EEA;
    text-align: center;
}

.close {
    background-color: #667EEA;
    width: 62px;
    height: 62px;
    border-radius: 62px;
    align-items: center;
    display: flex;    
    margin-top: 40px;
}

input {
    background-color: #a1c2dd;
    border: none;
    padding: 10px 15px;
    margin: 10px 0;
    width: 90%;
    border-radius: 9px;
    text-transform: uppercase;
}

img {
    width: 22px;
    height: 22px;
}

li {
    padding: 25px 0;
    font-size: 20px;
    font-weight: bold;
    color: #667EEA;
    margin-left: 5%;
    list-style: none;
    text-transform: uppercase;
}

input::placeholder{
    color: white;
    font-size: 15px;
}

.close span{
    color: white;
    font-size: 30px;
}
</style>