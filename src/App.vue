<template>
  <div id="app">
    <Select>
      <SelectOption></SelectOption>
    </Select>
  </div>
</template>

<script>
import Select from './components/Select.vue'
import SelectOption from './components/SelectOption.vue'

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
  padding: 100px;
}
</style>