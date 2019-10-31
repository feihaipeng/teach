<template>
  <div class="header_div">
    <div class="system_name">{{ name }}</div>
  </div>
</template>
<script>
export default {
  props: [ 'name' ]
}
</script>
<style lang="scss" scoped>
.header_div {
  width: 100%;
  height: 60px;
  @include bg_color($background-color-theme);
  .system_name {
    width: 200px;
    margin: 0 auto;
    text-align: center;
    font-size: 24px;
    @include font_color($font-color-theme)
  }
}
</style>
