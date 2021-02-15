<template>
  <button>
    <div>
      <img src="../assets/img/fin.png" alt="plusevenement">
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
    height: 60px;
    width: 20%;
    border-radius: 37px;
    border: solid 1px #707070;
    background-color: #6e66c8;
    display: flex;
    justify-content: space-evenly;
    padding-top: 9px;
  }

  button p {
    padding-top: 7px;
    font-size: 20px;
    font-weight: bold;
    color: #fafafd;
    text-transform: uppercase;
  }

  @media screen and (max-width: 1530px) {
    button p {
      padding-top: 10px;
      font-size: 15px;

    }
  }

  @media screen and (max-width: 1210px) {
    button p {
      padding-top: 13px;
      font-size: 12px;

    }
  }

  @media screen and (max-width: 1020px) {
    button {
      width: 30%;
    }

    button p {
      padding-top: 10px;
      font-size: 15px;

    }
  }

  @media screen and (max-width: 824px) {
    button {
      width: 40%;
    }

    button p {
      padding-top: 10px;
      font-size: 15px;

    }
  }

  @media screen and (max-width: 610px) {
    button {
      width: 50%;
    }
  }

  @media screen and (max-width: 500px) {
    button {
      width: 50%;
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