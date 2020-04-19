<template>
  <div id="wrapper">
    <main>
      <Layout></Layout>
    </main>
  </div>
</template>

<script>
  import Layout from './IndexPage/Layout'

  export default {
    name: 'landing-page',
    components: { Layout },
    methods: {
      open (link) {
        this.$electron.shell.openExternal(link)
      }
    }
  }
</script>

<style>

</style>
