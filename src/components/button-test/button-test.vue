<template>
  <div class="btn-wrap">
    <cube-button type="submit" icon="cubeic-right">Button</cube-button>
    <cube-button :light="true">Light Button</cube-button>
    <cube-button :inline="true">Inline Button</cube-button>
    <cube-button :outline="true">Outline Button</cube-button>
    <cube-button :primary="true">Primary Button</cube-button>
    <div class="tab">
      <ul>
        <li>标题一</li>
        <li>标题二</li>
        <li>标题三</li>
      </ul>
    </div>
    <cube-button @click="$refs.tip.show()">Show tip</cube-button>
    <cube-tip ref="tip" direction="bottom">Tip</cube-tip>
  </div>
</template>

<script>
  export default {
    name: 'button-test'
  }
</script>

<style scoped lang="stylus">
  @import "~@common/stylus/variable"
  .tab
    width: 100%;
    height: 36px;
    ul
      display flex
      justify-content space-around
      background-color $color-blue
      li
        font-size $fontsize-medium
        color: $color-col-line
        text-align center
        line-height: 36px
        background-color: $color-background-ss
        padding 0 12px
</style>
