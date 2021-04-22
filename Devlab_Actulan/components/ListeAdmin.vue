<template>
    <table>
        <tr>
            <th class="dark">Id</th>
            <th class="normal">PSEUDO</th>
            <th class="dark">EMAIL</th>
            <th class="normal">DROITS</th>
            <th class="dark">DERNIERE CONNEXION</th>
        </tr>
        <tr>
            <td class="normal">1</td>
            <td class="light">AYOUB9360</td>
            <td class="normal">ayoub.elguendouz@gmail.com</td>
            <td class="light"></td>
            <td class="normal"></td>
        </tr>
        <tr>
            <td class="normal">2</td>
            <td class="light">SAMY92xxx</td>
            <td class="normal">Samy.mahmoudi@gmail.com</td>
            <td class="light"></td>
            <td class="normal"></td>
        </tr>
    </table>

</template>

<script>

</script>

<style scoped>
    table {
        border-collapse: collapse;
        border-radius: 1em;
        overflow: hidden;
        width: 100%;
    }

    th,
    td {
        padding: 1em;
        background: #ddd;
    }

    th {
        color: #6E66C8;
        font-size: 25px;
        font-weight: bold;
    }

    tr:first-child {
        text-transform: uppercase;
    }

    td {
        color: #4D4D4D;
        font-size: 17px;
        font-weight: bold;
    }

    .css-mine {
        margin-top: 2em;
        clear: both;
    }

    .dark {
        background-color: #D5D5D5;
    }

    .normal {
        background-color: #E2E2E2;
    }

    .light {
        background-color: #F0F0F0;
    }

    @media screen and (max-width: 900px) {
        th {
            font-size: 15px;
            padding: 0.8em;
        }

        td {
            font-size: 12px;
            padding: 0.8em;
        }
    }
</style>
