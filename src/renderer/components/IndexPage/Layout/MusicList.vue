<template>
    <div class="container">
        <MusicListItem v-for="i in show_nums"></MusicListItem>
    </div>
</template>

<script>
    import MusicListItem from "./MusicList/MusicListItem";
    export default {
        components: {
            MusicListItem
        },
        data () {
          return {
              show_nums: 10
          }
        },
        name: "MusicList"
    }
</script>

<style scoped>

</style>