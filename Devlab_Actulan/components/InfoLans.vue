<template>
    <table>
        <tr>
            <td></td>
            <td></td>
        </tr>

        <tr class="grey">
            <td>Date de début : </td>
            <td>05/12/20 à 09H30</td>
        </tr>

        <tr class="white">
            <td>Date de fin : </td>
            <td>06/12/09 à 19H00</td>
        </tr>

        <tr class="grey">
            <td>Site web : </td>
            <td>nantarena.net</td>
        </tr>

        <tr class="white">
            <td>Nombre de place : </td>
            <td>192 places</td>
        </tr>

        <tr class="grey">
            <td>Prix d'entrée : </td>
            <td></td>
        </tr>

        <tr class="white">
            <td>Organisé par : </td>
            <td>Club Zéro</td>
        </tr>

        <tr class="grey">
            <td>Pays : </td>
            <td>France</td>
        </tr>

        <tr class="white">
            <td>Région : </td>
            <td>Pays de la Loire</td>
        </tr>

        <tr class="grey">
            <td>Département : </td>
            <td>Loire-Atlantique</td>
        </tr>

        <tr class="white">
            <td>Ville : </td>
            <td>Nantes (44300)</td>
        </tr>

        <tr class="grey">
            <td>Adresse : </td>
            <td>Rue Christian Pauc</td>
        </tr>

        <tr>
            <td></td>
            <td></td>
        </tr>
    </table>
</template>

<script>

</script>

<style scoped>
    table {
        border-collapse: collapse;
        border-radius: 13px;
        overflow: hidden;
        width: 100%;
    }

    th,
    td {
        padding: 0.3em;
    }

    tr {
        height: 70px;
    }

    body {
        margin: 1.5em;
    }

    .grey {
        background-color: rgb(170, 170, 170, 0.65);
    }

    .white {
        background-color: #F4F3F3;
    }

    td:first-child {
        color: #020202;
        font-size: 37px;
        font-weight: bold;
        text-align: initial;
        text-transform: uppercase;
    }

    td:last-child {
        color: #6E66C8;
        font-size: 20px;
        font-weight: 500;
        text-align: end;
    }

    tr:first-child,
    tr:last-child {
        background-color: #ffffff;
    }

    @media screen and (max-width: 1120px) {

        .left {
            font-size: 27px;
        }

        .right {
            font-size: 12px;
        }

    }
</style>
