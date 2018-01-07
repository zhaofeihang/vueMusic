<template>
  <div class="loading">
    <img src="./loading.gif" class="img">
    <p class="desc">{{title}}</p>
  </div>
</template>

<script>
    export default {
      props: {
        title: {
          type: String,
          default: '正在载入...'
        }
      }
    }
</script>

<style scoped lang="stylus" rel="stylesheet/stylus">
  @import '~common/stylus/variable'

  .loading
    text-align: center
    width: 100%
  .img
    width: 24px
    height: 24px
  .disc
    line-height: 20px
    font-size: $font-size-small
    color: $color-text-l
</style>
