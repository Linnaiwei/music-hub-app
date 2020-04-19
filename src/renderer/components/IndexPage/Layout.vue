<template>
  <section class="hero is-fullheight" id="Layout">
    <div class="hero-head">
      <MusicNav></MusicNav>
    </div>
    <div class="hero-body music-list-container">
      <MusicList></MusicList>
    </div>
    <div class="hero-foot">
      foot
    </div>
  </section>
</template>

<script>
  import MusicNav from "./Layout/MusicNav";
  import MusicList from "./Layout/MusicList";
  export default {
    components: {
      MusicNav,
      MusicList
    },
    data () {
      return {
        electron: process.versions.electron,
        name: this.$route.name,
        node: process.versions.node,
        path: this.$route.path,
        platform: require('os').platform(),
        vue: require('vue/package.json').version
      }
    }
  }
</script>

<style lang="less" type="text/less" scoped>
  #Layout{
    .music-list-container{
      align-items: stretch;
    }
  }
</style>
