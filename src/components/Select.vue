<template>
<div class="select">
  <div class="input-wrapper">
    <input type="text" :value="value">
  </div>
  <div class="option-wrapper">
    <slot>
      
    </slot>
  </div>
</div>
</template>
<script>
export default {
  name: 'Select',
  data() {
    return {
      value: ''
    }
  }
}
</script>
<style scoped lang="scss">
  
</style>
