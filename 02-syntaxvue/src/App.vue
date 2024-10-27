<script setup>
const message = 'hello world'; // binding data
const rawHtml = '<span style="color: red">This should be red.</span>'; // raw html
const buttonId = 'button-id'; // binding attribute
const buttonClass = 'btn btn-rounded'; // binding class
const isButtonDisabled = false; // binding disabled
const objectOfAttributes = { // binding attributes
  id: 'button-id',
  class: 'wrapper'
}

const number = 0; // binding expression 
</script>

<template>
  <h1>Hello World</h1>
  <p>Message: {{ message }}</p>
  <p v-html="rawHtml"></p>
  <button :id="buttonId" :class="buttonClass" :disabled="isButtonDisabled"> {{isButtonDisabled ? 'Disable' : 'Click here'}}</button>
  <button v-bind="objectOfAttributes"> Click here</button>

  <button>Number: {{ number }}</button>

</template>
