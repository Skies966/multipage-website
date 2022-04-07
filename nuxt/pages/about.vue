<template>
  <div>
    <TheHeader>
    </TheHeader>
  
    <TheFooter>
    </TheFooter>
  </div>
</template>

<script setup>
export default {
  data: () => ({
    posts: []
  }),
  async fetch() {
    this.posts = await this.$http.$get('https://api.nuxtjs.dev/posts')
  },
  fetchOnServer: false,
  // multiple components can return the same `fetchKey` and Nuxt will track them both separately
  fetchKey: 'site-sidebar',
  // alternatively, for more control, a function can be passed with access to the component instance
  // It will be called in `created` and must not depend on fetched data
  fetchKey(getCounter) {
    // getCounter is a method that can be called to get the next number in a sequence
    // as part of generating a unique fetchKey.
    return this.someOtherData + getCounter('sidebar')
  }

</script>

<style>

</style>