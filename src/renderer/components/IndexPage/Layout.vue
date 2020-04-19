<template>
  <section class="hero is-fullheight">
    <div class="hero-head">
      <MusicNav></MusicNav>
    </div>
    <div class="hero-body">
      body
    </div>
    <div class="hero-foot">
      foot
    </div>
  </section>
</template>

<script>
  import MusicNav from "./Layout/MusicNav";
  export default {
    components: {
      MusicNav
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

<style scoped>

</style>
