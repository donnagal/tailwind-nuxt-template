<template>
  <div>
    <Navbar />
    <nuxt />
  </div>
</template>

<script>
  import Navbar from '@/components/Navbar'

  export default {
    components: {
      Navbar
    }
  }
</script>


<style>
  html {
    font-family: 'Quicksand', 'Source Sans Pro', -apple-system, BlinkMacSystemFont,
      'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
    font-size: 16px;
    word-spacing: 1px;
    -ms-text-size-adjust: 100%;
    -webkit-text-size-adjust: 100%;
    -moz-osx-font-smoothing: grayscale;
    -webkit-font-smoothing: antialiased;
    box-sizing: border-box;
  }
  h1  { @apply font-bold text-5xl pb-1;}
  h2  { @apply font-bold text-3xl pb-1;}
  h3  { @apply font-bold text-2xl pb-1;}
  p   { @apply text-lg text-gray-600  pb-8;}
  .lead { @apply text-2xl text-gray-500  pb-5;}

  button {@apply bg-black font-bold text-white uppercase text-sm px-6 py-4;}
</style>
