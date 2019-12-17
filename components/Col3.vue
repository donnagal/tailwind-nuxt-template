<template>
<div class="bg-gray-200 pb-24">
    <div class="container mx-auto">
      <div class="p-5">
        <h3 class="mark-bold text-4xl uppercase">Three column block</h3>
      </div>
      <div class="flex items-center flex-wrap uppercase text-center text-xs text-gray-700 tracking-wider aos-init aos-animate" data-aos="fade" data-aos-easing="ease-in" data-aos-duration="500">
          <div class="lg:w-1/3 px-5">
            <img src="https://images.unsplash.com/photo-1576017357802-09adcbd17779?ixlib=rb-1.2.1&amp;ixid=eyJhcHBfaWQiOjEyMDd9&amp;auto=format&amp;fit=crop&amp;w=500&amp;q=60">
            <p class="pt-2 pb-10">colour pop</p>
          </div>
          <div class="lg:w-1/3 px-5">
            <img src="https://images.unsplash.com/photo-1558981285-6f0c94958bb6?ixlib=rb-1.2.1&amp;ixid=eyJhcHBfaWQiOjEyMDd9&amp;auto=format&amp;fit=crop&amp;w=500&amp;q=60">
            <p class="pt-2 pb-10">Harley-Davidson</p>
          </div>
          <div class="lg:w-1/3 px-5">
            <img src="https://images.unsplash.com/photo-1540228510585-5f95da870c80?ixlib=rb-1.2.1&amp;ixid=eyJhcHBfaWQiOjEyMDd9&amp;auto=format&amp;fit=crop&amp;w=800&amp;q=60">
            <p class="pt-2 pb-10">Underground</p>
          </div>
      </div>

    </div>
  </div>
</template>

<script>
export default {
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

</style>
