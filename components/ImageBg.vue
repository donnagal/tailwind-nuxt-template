<template>
  <div class="bg-auto bg-center bg-cover" 
   :style="{ backgroundImage: `url(${backgroundUrl})` }">
    <div class="overlay"></div>
    <div class="flex lg:content-center lg:pt-0 flex-wrap h-screen">
      <div class="container mx-auto px-10 lg:px-0 z-10">
          <div class="lg:w-1/3 text-white" data-aos="fade-up">
            <h4 class="uppercase">{{this.subtitle}}</h4>
            <h1 class="mb-8 mark-bold lg:text-6xl text-5xl leading-none">
             {{this.title}}
            </h1>
            <button class="bg-white font-bold text-black uppercase text-sm px-6 py-4 hover:opacity-75">Get started</button>
          </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  mounted() {
    AOS.init();
  },
    props: {
      title: {
        type: String,
      },
      subtitle: {
        type: String,
      },
      backgroundUrl: {
         type: String,
      }
    },
}
</script>


<style scoped>
  p {@apply text-white;}
  .overlay {@apply absolute w-full h-full bg-gray-900 opacity-50 top-0 left-0;}
</style>
