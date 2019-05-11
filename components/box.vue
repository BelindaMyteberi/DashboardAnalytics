<template>
  <div class="header-container">
    <input type="text" name="write" v-model="valueOfInput">
    <h3 id="input_written">
      <span> {{valueOfInput}}</span>
    </h3>
  </div>
</template>
<script>
  export default {
    data() {
      return {
        valueOfInput: ''
      }
    },

    methods: {
      getValue () {
        console.log(this.display)
      }
    }
  }
</script>
<style lang="scss">

</style>
