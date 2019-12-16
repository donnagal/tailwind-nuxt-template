<template>
  <div>
    <ImageBg title="Blog" backgroundUrl='https://images.unsplash.com/photo-1573844077939-8eabe5be728f?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=1500&q=80'/>
    <div class="container mx-auto pt-10 pb-24">
      <h1>Edtions</h1>
        <ul class="list-disc list-inside">
          <li><nuxt-link :to="`/posts/blog`">Blog</nuxt-link></li>
          <li><nuxt-link :to="`/posts/blog-1`">Blog 1</nuxt-link></li>
          <li><nuxt-link :to="`/posts/blog-2`">Blog 2</nuxt-link></li>
      </ul>
    </div>
  </div>
</template>

<script>
import ImageBg from '~/components/ImageBg.vue'

export default {
  components: {
    ImageBg
  }
}
</script>

<style>
  li {@apply underline text-xl pb-4;}
</style>
