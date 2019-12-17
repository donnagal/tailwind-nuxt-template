<template>
  <div>
      <ImageBg title="North Shore of Oahu, Hawaii." subtitle="North Shore, Waialua, United States"  backgroundUrl='https://images.unsplash.com/photo-1507525428034-b723cf961d3e?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=1506&q=80'/>
      
      <div class="container mx-auto pt-10 pb-24">
      <h1>This is Page 1</h1>
      <p class="lead">Lorem, ipsum dolor sit amet consectetur adipisicing elit. Porro praesentium voluptates quam optio vel pariatur consectetur nesciunt excepturi incidunt delectus, facilis atque quaerat libero quod perferendis. Reprehenderit aliquid natus inventore.</p>
      
      <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Quibusdam omnis repudiandae dolorum,
         natus sed commodi molestias incidunt saepe accusantium a facere quaerat tempore nemo doloribus 
         aut voluptas? Tenetur, delectus aperiam. This is <a class="underline" href="#">a link here</a>.
      </p>

     <button class="hover:opacity-75">Button default</button>

    </div>
      <Col3 />
  </div>
</template>

<script>
import ImageBg from '~/components/ImageBg.vue'
import Col3 from '~/components/Col3.vue'

export default {
  components: {
    ImageBg,
    Col3
  },
}
</script>





<style scoped>

</style>
