<template>
  <label class="label-checkbox"> News
    <input type="checkbox" checked="checked">
    <span class="checkmark"></span>
</template>

<script>

</script>

<style scoped>
  /* The container */
  .label-checkbox {
    display: block;
    position: relative;
    padding-left: 60px;
    padding-top: 5px;
    margin-bottom: 12px;
    cursor: pointer;
    font-size: 22px;
  }

  /* Hide the browser's default checkbox */
  .label-checkbox input {
    position: absolute;
    opacity: 0;
    cursor: pointer;
    height: 0;
    width: 0;
  }

  /* Create a custom checkbox */
  .checkmark {
    position: absolute;
    top: 0;
    left: 0;
    width: 40px;
    height: 40px;
    background-color: #eee;
    border: 2px solid black;
    border-radius: 10px;
  }

  /* On mouse-over, add a grey background color */
  .label-checkbox:hover input~.checkmark {
    background-color: #ccc;
  }

  /* When the checkbox is checked, add a blue background */
  .label-checkbox input:checked~.checkmark {
    background-color: #6e66c8;
    border-radius: 10px;
    border: none;
    width: 40px;
    height: 40px;
  }

  /* Create the checkmark/indicator (hidden when not checked) */
  .checkmark:after {
    content: "";
    position: absolute;
    display: none;
  }

  /* Show the checkmark when checked */
  .label-checkbox input:checked~.checkmark:after {
    display: block;
  }

  /* Style the checkmark/indicator */
  .label-checkbox .checkmark:after {
    left: 13px;
    top: 5px;
    width: 10px;
    height: 20px;
    border: solid white;
    border-width: 0 3px 3px 0;
    -webkit-transform: rotate(45deg);
    -ms-transform: rotate(45deg);
    transform: rotate(45deg);
  }
</style>