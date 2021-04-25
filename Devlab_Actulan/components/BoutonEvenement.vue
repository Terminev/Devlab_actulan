<template>
  <button>
    <div>
      <span>+</span>
    </div>
    <p>{{ Text }}</p>
  </button>
</template>

<script>
export default{
    props: ["Text"]
}
</script>

<style scoped>
  button {
    border-radius: 37px;
    border: solid 1px #707070;
    background-color: #6E66C8;
    display: flex;
    justify-content: space-evenly;
    padding: 15px 40px;
  }

  button:hover{
    cursor: pointer;
  }

  button p {
    padding: 7px 64px 0px 75px;
    font-size: 20px;
    font-weight: bold;
    color: #fafafd;
    text-transform: uppercase;
  }

  div{
    border-radius: 50px;
    box-shadow: 0 4px 20px 0 rgba(0, 0, 0, 0.81);
    background-color: #f9f8fa;
    width: 35px;
    height : 35px;
  }

  span{
     font-size: 22px;
    font-weight: bold;
     color: #6e66c8;
     text-align: center;
     display: block;
     padding-top: 4px;
  }

  @media screen and (max-width: 488px) {
    button p {
      padding: 5px 25px 0px 25px;
      font-size: 19px;
       text-transform: initial;
    }

    button {
     border-radius: 10px;
      padding: 10px 20px;
    }
  }

  @media screen and (max-width: 488px) {
    button {
      width: 80%;
    }
  }

  @media screen and (max-width: 302px) {
    button {
      width: 100%;
    }
  }
</style>
