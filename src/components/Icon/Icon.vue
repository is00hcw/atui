<template>
<i :class="[prefixCls + '-iconfont', prefixCls + '-icon-' + type]" :style="{ fontSize: size + 'px',color:color }">
  <slot></slot>
</i>
</template>

<script>
export default {
  name: 'Icon',
  props: {
    type: {
      type: String,
      require: true
    },
    size: {
      type: String
    },
    color: {
      type: String
    },
    prefixCls: {
      type: String,
      default: 'atui'
    }
  }
}
</script>
