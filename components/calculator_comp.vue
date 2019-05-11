<template>
  <div>
    <div class="input-container">
      <input type="number" v-model="valueOfInput1">

      <select id="values" v-model="operator">
        <option value="+">+</option>
        <option value="-">-</option>
        <option value="/">/</option>
        <option value="*"> * </option>
      </select>
      <input type="number" v-model="valueOfInput2">
    </div>
    <div>
      <button id="button" @click="calculateSum">Click me </button>
      <p> Show Result: </p>
      <p> {{result}}</p>
    </div>
  </div>
</template>
<script>
  export default {
    data() {
      return {
        valueOfInput1:0,
        valueOfInput2:0,
        result: 0,
        operator: '',
      }
    },

    methods: {
     calculateSum () {
       this.result = `${this.valueOfInput1} ${this.operator} ${this.valueOfInput2}`
       // this.result = this.valueOfInput1 + this.valueOfInput2
     }
    }
  }
</script>
