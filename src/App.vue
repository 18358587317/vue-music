<template>
  <div id="app">
    <div class="background">
      <img width="100%" height="100%" src="~common/image/sky.jpg">
    </div>
    <m-header></m-header>
    <tab></tab>
    <keep-alive>
      <router-view></router-view>
    </keep-alive>
    <player></player>
  </div>
</template>

<script>
import MHeader from 'components/m-header/m-header'
import Tab from 'components/tab/tab'
import Player from './components/player/player'
export default {
  name: 'App',
  components: {
    Player,
    MHeader,
    Tab
  }
}
</script>

<style scoped lang="stylus" rel="stylesheet/stylus">
.background
  position: fixed
  left: 0
  top: 0
  width: 100%
  height: 100%
  z-index: -1
  opacity: 1
  filter: blur(5px)
</style>
