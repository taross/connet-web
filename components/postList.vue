<template>
  <div>
    <el-card v-for="(post,index) in posts" :key="index">
      <span>{{ post.userId }}</span><br/>
      <span>
        {{ post.message}}
      </span>

    </el-card>
  </div>
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

<style scoped>

</style>
