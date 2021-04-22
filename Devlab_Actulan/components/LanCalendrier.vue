<template>
  <div>
    <span>
      <p>{{ date }}</p>
      <h5>{{ titre }}</h5>
    </span>
    <p>{{ place }}</p>
  </div>
</template>

<script>
  export default{
    name: 'LanCalendrier',
    props: ["date", "titre", "place"]
  }
</script>

<style scoped>
  div {
    border: black solid 2px;
    display: flex;
    flex-wrap: nowrap;
    align-items: center;
    background-color: white;
    justify-content: space-between;
    padding: 5px 10px;
  }

  span{
    display: flex;
    align-items: center;
  }

  h5 {
    text-transform: uppercase;
    font-size: 22px;
    margin-left: 30%;
    font-weight: 500;
  }

  p:first-child {
    margin-left: 10px;
    background-color: #6E66C8;
    padding: 18px 8px;
    color: white;
    font-size: 15px;
    font-weight: bold;
    border-radius: 50px;
  }

  p:last-child {
    font-size: 16px;
    margin: 20px;
    text-transform: uppercase;
  }

  @media screen and (max-width: 1024px) {
    p:first-child {
      font-size: 12px;
      padding: 16px 8px;
    }

    p:last-child {
      font-size: 14px;
    }

    h5 {
      font-size: 18px;
      margin-left: 15%;
    }
  }

  @media screen and (max-width: 901px) {
    div {
      box-shadow: 0 3px 6px 0 rgba(0, 0, 0, 0.16);
      background-color: #d8d5d5;
      border: none;
      height: 40px;
      border-radius: 13px;
    }

    p {
      margin: 0;
      font-size: 14px;
    }

    p:first-child {
      margin-left: -15px;
    }

    p:last-child {
      display: flex;
      justify-content: flex-end;
      margin: 10px;
    }
  }
</style>
