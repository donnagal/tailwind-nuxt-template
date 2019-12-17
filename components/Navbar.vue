<template>
  <nav class="">

    <div class="block lg:hidden m-1 absolute left-0">
        <button class="button-m flex items-center px-3 py-2 border rounded text-white border-white hover:text-white hover:border-white">
          <svg class="fill-current h-3 w-3" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><title>Menu</title><path d="M0 3h20v2H0V3zm0 6h20v2H0V9zm0 6h20v2H0v-2z"/></svg>
        </button>
    </div>
      
<div class="menu hidden lg:block">
    <div class="bg-gray-900 lg:bg-transparent flex flex-wrap content-center w-full lg:py-10 text-white text-center"> 
  
    <div class="lg:w-1/3 w-full">
      <Logo />
    </div>
    
    <div class="lg:w-1/3 w-full">
      <nuxt-link :to="{name: 'index'}">Home</nuxt-link>
      <nuxt-link :to="`/page1`">Next Page</nuxt-link>
      <nuxt-link :to="`/posts/post`">Blogs</nuxt-link>
    </div>
  
    <div class="lg:w-1/3 w-full">
      <button class="bg-white w-full lg:w-auto font-bold text-black uppercase text-sm px-6 py-4 hover:opacity-75">Get started</button>
    </div>
  </div>
</div>
  
</nav>

</template>


<script>
  import Logo from '~/components/Logo.vue'

  export default {
    components: {
      Logo
    },
  }
</script>


<style>
  nav { @apply absolute top-0 w-full z-10;}
  nav a { @apply mx-4 uppercase; }
  nav svg { height: 50px; }

</style>
