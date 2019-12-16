<template>
  <div>
      <ImageBg title="Nuxt Template" subtitle="Welcome to the"  backgroundUrl='https://images.unsplash.com/photo-1547381496-57b53693e8e4?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=2090&q=80'/>
      <div class="container mx-auto pt-10 pb-24">
      <h1>Vue | Nuxt Template</h1>
      <p class="lead">Lorem, ipsum dolor sit amet consectetur adipisicing elit. Porro praesentium voluptates quam optio vel pariatur consectetur nesciunt excepturi incidunt delectus, facilis atque quaerat libero quod perferendis. Reprehenderit aliquid natus inventore.</p>
      
      <h2>Nuxt?</h2>
      <p>With Nuxt.js, your application will be optimized out of the box. We do our best to build performant applications by utilizing Vue.js and Node.js best practices. To squeeze every unnecessary bit out of your app Nuxt includes a bundle analyzer and lots of opportunities to fine-tune your app.</p>

      <h3>Why we need design systems</h3>
      <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Quibusdam omnis repudiandae dolorum,
         natus sed commodi molestias incidunt saepe accusantium a facere quaerat tempore nemo doloribus 
         aut voluptas? Tenetur, delectus aperiam. This is <a class="underline" href="#">a link here</a>.
      </p>

     <button class="hover:opacity-75">Button default</button>

    </div>
  </div>
</template>

<script>
import ImageBg from '~/components/ImageBg.vue'

export default {
  components: {
    ImageBg
  },
}
</script>





<style scoped>

</style>
