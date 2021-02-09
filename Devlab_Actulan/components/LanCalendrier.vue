<template>
  <div>
    <span>
      <p>{{ date }}</p>
      <p>{{ titre }}</p>
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
    width: 80%;
    height: 70px;
    justify-content: space-between;
  }

  p {
    margin-left: 10%;
    text-transform: uppercase;
  }

  span{
    display: flex;
    align-items: center;
  }

  span p:first-child {
    margin-left: 10px;
    background-color: #6e66c8;
    padding: 16px 8px;
    color: white;
    font-size: 16px;
    font-weight: bold;
    border-radius: 50px;
  }

  p:last-child {
    margin: 20px;
  }

  @media screen and (max-width: 1375px) {
    div {
      width: 90%;
    }
  }

  @media screen and (max-width: 1024px) {
    p {
      font-size: 14px;
    }
  }

  @media screen and (max-width: 901px) {
    div {
      box-shadow: 0 3px 6px 0 rgba(0, 0, 0, 0.16);
      background-color: #d8d5d5;
      border: none;
      width: 70%;
      height: 40px;
      border-radius: 13px;
    }

    p {
      margin: 0;
      font-size: 14px;
    }

    span p:first-child {
      margin-left: -15px;
    }

    p:last-child {
      display: flex;
      justify-content: flex-end;
      margin: 10px;
    }
  }

  @media screen and (max-width: 500px) {
    div {
      width: 100%;
    }
  }
</style>
