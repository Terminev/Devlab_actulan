<template>
    <form action="">
        <label for="Rechercher">
            <input type="search" placeholder="Rechercher un organisme">
            <button type="submit">
                <img src="img/loupe.png" alt="loupe" id="loupe">
            </button>
        </label>
    </form>
</template>

<script>
    
</script>

<style scoped>
    form {
        align-items: center;
        background-color: white;
        border: solid 1px black;
        height: 50px;
        width: 450px;
        display: flex;
        justify-content: space-between;
        border-radius: 13px;
        align-items: center;
    }

    form label {
        display: flex;
    }

    input {
        width: 400px;
        padding: 10px;
        border-style: none;
        font-weight: 500;
        outline: none;
        font-size: 20px;
    }

    button {
        border-style: none;
        background-color: white;
    }

    input::placeholder {
        color: #6E66C8;
        font-size: 20px;
    }
</style>