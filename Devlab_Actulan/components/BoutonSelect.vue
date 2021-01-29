<template>
<select name="">
        <option value="Supports">Supports</option>
        <option value="dog">Dog</option>
        <option value="cat">Cat</option>
        <option value="hamster">Hamster</option>
        <option value="parrot">Parrot</option>
        <option value="spider">Spider</option>
        <option value="goldfish">Goldfish</option>
    </select>
</template>

<script>

</script>

<style scoped>
    select {
        height: 50px;
        width: 20%;
        font-weight: 500;
        color: #fdfafa;
        font-size: 22px;
        background-color: #6e66c8;
        border-radius: 20px;
    }

    option {
        background-color: #9d94ff;

    }

    @media screen and (max-width: 900px) {
        select {
            width: 50%;

        }
    }

    @media screen and (max-width: 425px) {
        select {
            width: 100%;

        }
    }
</style>