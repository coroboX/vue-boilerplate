<template>
  <div>
    <h1>{{ msg }}</h1>
  </div>

</template>

<script>
import Vue from 'vue'
const buttonCounterComponent = Vue.component('button-counter', {
  data: function () {
    return {
      count: 0
    }
  },
  template: '<button v-on:click="count++">You clicked me {{ count }} times.</button>'
})

export default {
  components: {
    'button-counter': buttonCounterComponent
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
