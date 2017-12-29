<template>
  <div>
    <Header/>
    <div class="tab">
      <div class="tab-item">
        <router-link class="router-link" to="/goods">商品</router-link>
      </div>
      <div class="tab-item">
        <router-link class="router-link" to="/ratings">评论</router-link>
      </div>
      <div class="tab-item">
        <router-link class="router-link" to="/seller">商家</router-link>
      </div>
    </div>
    <router-view/>
  </div>
</template>

<script>
import Header from './components/header/header'

export default {
  name: 'app',
  components: {
    Header
  }
}
</script>

<style lang="stylus" rel="stylesheet/stylus">
  .tab{
    display: flex
    width: 100%
    height: 40px
    line-height: 40px
  }
  .tab .tab-item{
    flex: 1
    text-align: center
  }
  .tab .tab-item .router-link{
    display: block
    text-decoration: none
  }
</style>
