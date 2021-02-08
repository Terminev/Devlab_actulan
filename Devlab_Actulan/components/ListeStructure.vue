<template>
  <table>
    <tr>
      <th>{{ Nom }}</th>
      <th class="border">{{ Lieux }}</th>
      <th>{{ Lans }}</th>
    </tr>

    <tr class="white">
      <td>{{ Nom1 }}</td>
      <td>{{ Lieux1 }}</td>
      <td>{{ Lans1 }}</td>
    </tr>
    <tr class="grey">
      <td>{{ Nom2 }}</td>
      <td>{{ Lieux2 }}</td>
      <td>{{ Lans2 }}</td>
    </tr>
  </table>
</template>

<script>
export default {
  name: "ListeStructure",
  props: [
    "Nom",
    "Lieux",
    "Lans",
    "Nom1",
    "Lieux1",
    "Lans1",
    "Nom2",
    "Lieux2",
    "Lans2",
  ],
};
</script>

<style scoped>
table {
  border-collapse: collapse;
  overflow: hidden;
  text-align: center;
}

th,
td {
  padding: 1em;
}

th {
  background-color: #02010b;
  color: #ffffff;
  font-size: 20px;
  font-weight: normal;
  width: 1%;
  text-transform: uppercase;
}

td {
  color: #000000;
  font-size: 20px;
  font-weight: normal;
}

.css-mine {
  margin-top: 2em;
  clear: both;
}

.white {
  background-color: #ffffff;
}

.grey {
  background-color: #f4f3f3;
}

.border {
  border-right: solid 1px white;
  border-left: solid 1px white;
}

td:first-child {
  text-align: left;
}

@media screen and (min-width: 319px) and (max-width: 899px) {
  th {
    font-size: 7px;
  }

  td {
    font-size: 12px;
  }
}
</style>
