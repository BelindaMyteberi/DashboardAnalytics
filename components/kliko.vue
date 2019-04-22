<template>
  <div class="header-container">
    <button @click="getValue">Kliko</button>
  </div>
</template>
<script>
  export default {
    data() {
      return {
        display: 'Shfaq'
      }
    },
    methods: {
      getValue () {
        console.log(this.display)
      }
    }
  }
</script>
