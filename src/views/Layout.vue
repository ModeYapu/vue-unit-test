<template>
  <div class="page">
    <p>Layout</p>
    <span>固定自适应布局</span>
    <div class="content">
      <div class="left"></div>
      <div class="right"></div>
    </div>
    <span>垂直居中布局 flex</span>
    <div class="content1">
      <div class="center"></div>
    </div>
    <span>垂直居中布局2 transform</span>
    <div class="content2">
      <div class="center"></div>
    </div>
    <span>垂直居中布局3 table</span>
    <div class="warb">
      <div class="content3">
        <div class="center"></div>
      </div>
    </div>
  </div>
</template>

<style lang="stylus" scoped>
.page
  width 100%
  height 100%
  margin 0
  padding 0
  .content
    height 40px
    width 100%
    display flex
    background-color #e3e3e3
    .left
      width 30px
      background #eeeeee
  .content1
    width 100%
    height 300px
    display flex
    align-items center
    justify-content center
    background-color #f5f5f5
    .center
      height 20px
      width 50px
      background-color #e2e2e2
  .content2
    width 100%
    height 200px
    position relative
    background-color #f5f5f5
    .center
      height 20px
      width 50px
      position absolute
      left 50%
      top 50%
      transform translate(-50%, -50%)
      background-color #e2e2e2
  .warb
    display table
    width 100%
    height 200px
    .content3
      display table-cell
      vertical-align middle
      background-color #f5f5f5
      .center
        height 20px
        width 50px
        margin auto
        text-align center
        background-color #e2e2e2
</style>