<template>
<div class="select">
  <div class="input-wrapper">
    <input type="text" :value="value" :readonly="readonly"
      @change="$emit('change', $event.target.value)"
      @input="$emit('input', $event.target.value)"
      @focus="$emit('focus', $event.target.value)"
      @blur="$emit('blur', $event.target.value)"
    >
    <i class="iconfont vicon-select"></i>
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
      readonly: true
    }
  },
  props: {
    value: {
      type: String,
      required: true
    }
  }
}
</script>
<style scoped lang="scss">
$font-size: 14px;
  div, input {
    box-sizing: border-box;
    padding: 0;
    margin: 0;
  }
  .select {
    display: inline-flex;
    justify-content: center;
    align-items: center;

    position: relative;
    width: 100%;
    min-width: 200px;
    height: 100%;
    min-height: 24px;
    border: 1px solid red; // FIXME delete it
    font-size: $font-size;
    background: transparent;
    cursor: pointer;
    .input-wrapper {
      width: 100%;
      height: 100%;
      display: inline-flex;
      justify-content: center;
      align-items: center;
      input {
        width: 100%;
        height: 100%;
        border: none;
        font-size: $font-size;
        padding-right: 24px;
        background: transparent;
        cursor: pointer; 
        &:focus {
          outline: none;
        }
      }
      .iconfont {
        background: transparent;
        position: absolute;
        font-size: 14px;
        right: 0;
        width: 24px;
      }
    }
    &:hover {
      background-color: #20292b;
    }
  }
</style>
