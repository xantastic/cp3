<template>
  <div>
    <h1>PlayLists</h1>
    <PlayListList :playList="PlayListProp" />
  </div>
</template>

<script>
import PlayListList from "../components/PlayListList.vue";
export default {
  name: "Playlist",
  components: {
    PlayListList,
  },
  computed: {
      PlayListProp() {
          return this.$root.$data.playlists;
      }
  }
  

};
</script>

<style scoped>
  h1 {
    color: white;
  }
</style>
