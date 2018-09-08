<template>
  <ul>
    <li v-for="(post,index) in posts" :key="index">
      {{ post.id }}：{{ post.message }} @{{ post.userId }}
    </li>
  </ul>
</template>

<script>
  import { mapGetters } from 'vuex'
  export default {
    computed: {
      ...mapGetters({
        posts: 'getItems'
      })
    }
  }
</script>
