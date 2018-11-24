<template>
<div class="select">
  <div class="input-wrapper">
    <input type="text" :value="value" 
      @change="$emit('change', $event.target.value)"
      @input="$emit('input', $event.target.value)"
      @focus="$emit('focus', $event.target.value)"
      @blur="$emit('blur', $event.target.value)"
    >
  </div>
  <div class="option-wrapper">
    <slot slot="option">
      
    </slot>
  </div>
</div>
</template>
<script>
export default {
  name: 'Select',
  data() {
    return {
    }
  },
  props: {
    value: {
      type: String
    }
  }
}
</script>
<style scoped lang="scss">
  
</style>
