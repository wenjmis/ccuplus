<template>
  <div class="post-list">
    <div v-for="post in posts" :key="post.id">
      <SinglePost :post="post" />
    </div>
  </div>
</template>

<script>
// component imports
import SinglePost from './SinglePost.vue'
export default {
  props: ['posts'],
  components: { SinglePost },
  setup() {
  }
}
</script>

<style>

</style>