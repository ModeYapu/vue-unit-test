<template>
  <div class="page">
    <p>新的几个时间</p>
    <div class="wrapper">
      <div class="one">One</div>
      <div class="two">Two</div>
      <div class="three">Three</div>
      <div class="four">Four</div>
      <div class="five">Five</div>
      <div class="six">Six</div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang='stylus' scoped>
.page
  height 100%
  width 100%
  .wrapper
    display grid
    grid-template-columns repeat(4, 1fr)
    grid-gap 10px
    grid-auto-rows minmax(100px, auto)
    div
      border 2px solid rgb(233, 171, 88)
      border-radius 5px
      background-color rgba(233, 171, 88, 0.5)
      padding 1em
      color #d9480f
    .one
      grid-column 1 / 3
      grid-row 1
    .two
      grid-column 2 / 4
      grid-row 1 / 3
    .three
      grid-row 2 / 5
      grid-column 1
    .four
      grid-column 3
      grid-row 3
    .five
      grid-column 2
      grid-row 4
    .six
      grid-column 3
      grid-row 4
</style>