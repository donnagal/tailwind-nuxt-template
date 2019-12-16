<template>
  <div>
   <nav>
    <nuxt-link :to="{name: 'index'}">Home</nuxt-link>
    <nuxt-link :to="`/posts/post`">Blogs</nuxt-link>
  </nav>
  </div>
</template>


<script>
</script>


<style>
  nav {
    @apply w-full py-8 bg-gray-900 text-white text-center fixed top-0 z-50;
  }

</style>
