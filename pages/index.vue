<template>
  <div>
    <div class="posts">
      <post-list/>
    </div>


  </div>
</template>

<script>
  import { mapGetters } from 'vuex'
  import PostList from "../components/postList";
  export default {
    components: {PostList},
    computed: {
      ...mapGetters({
        posts: 'getItems'
      })
    }
  }
</script>

<style scoped>
  .posts{
    box-sizing: border-box;
    width: 40vw;
    margin-top: 2vh;
    margin-left: 2vw;
  }
</style>
