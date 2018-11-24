<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <Select>
      <SelectOption></SelectOption>
    </Select>
  </div>
</template>

<script>
import Select from './components/Select.vue'
import SelectOption from './components/Select.vue'

export default {
  name: 'app',
  components: {
    Select,
    SelectOption
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>