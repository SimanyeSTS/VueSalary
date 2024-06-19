<template>
  <form class="container">
    <input type="number" placeholder="Enter Rate" required v-model="rate">
    <input type="number" placeholder="Enter Hours" required v-model="hours"
    <input type="number" required v-model="salary">
    <button @click.prevent="salary">Calculate</button>
    <button @click.prevent="clear">Clear</button>
  </form>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'App',
  components: {

  },
  data() {
    return {
      rate: '',
      hours: '',
      output: 'rate' * 'hours'
    }
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
.container {
  display: grid;
  gap: .2rem;
  width: 30rem;
  margin-inline: auto;
  & input { 
    text-align: center;
  }
}
.rate {
  border: 2px solid;
}
.hours {
  border: 2px solid;
}
.salary {
  border: 2px solid;
}
</style>
