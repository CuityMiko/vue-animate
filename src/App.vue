<template>
  <div id="app">
    <div class="app-header">
      <top-nav></top-nav> 
    </div>
    <main class="app-content main-content">
      <router-view/>
    </main>
    <div class="app-footer">
      <footer-bar></footer-bar>
    </div>
    <side-bar></side-bar>
    <search-bar v-if="searchBar"></search-bar>
  </div>
</template>

<script>
import { mapState } from 'vuex'
import topNav from '@/components/topNav'
import footerBar from '@/components/footerBar'
import sideBar from '@/components/sideBar'
import searchBar from '@/components/searchBar'

export default {
  name: 'app',
  components: {
    topNav,
    footerBar,
    sideBar,
    searchBar
  },
  computed: mapState(['searchBar'])
}
</script>

<style lang="less" scoped>
.app-content {
  width: 100%;
  height: 28rem;
  // overflow: hidden;
  overflow: scroll;
  background-color: #fff;
}
.app-footer {
  width: 100%;
  position: fixed;
  bottom: 0;
}
</style>
