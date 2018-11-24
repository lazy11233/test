<template>
  <div id="app">
    <VSelect v-model="msg" style="width:200px; height: 32px;">
      <VSelectOption></VSelectOption>
    </VSelect>
    <button @click="changeMSG">
      .
    </button>
  </div>
</template>
<script>
import VSelect from './components/Select.vue'
import VSelectOption from './components/SelectOption.vue'

export default {
  name: 'app',
  components: {
    VSelect,
    VSelectOption
  },
  data() {
    return {
      msg: 'fadfa'
    }
  },
  methods: {
    changeMSG() {
      this.msg += 1;
    }
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