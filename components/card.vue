<template>
  <main class="bg-white">
    <div class=" grid grid-cols-1 sm:grid-cols-2 gap-x-20 gap-y-10 p-20 content-center ">
      <section class="">
        <h2 class="text-s font-bold text-blue-500">Deploy faster</h2>
        <h2 class="text-4xl font-bold text-black mb-4">{{ Title }}</h2>
        <p class="text-xl text-gray-600 mb-8">Lorem ipsum, dolor sit amet consectetur adipisicing elit. Maiores impedit
          perferendis suscipit eaque, iste dolor cupiditate blanditiis ratione.</p>
        <div class="pl-4">
          <p class="text-black mb-8"><strong><img src="https://cdn-icons-png.flaticon.com/512/218/218706.png"
                class="inline-block h-6 w-6 mr-2">Push to deploy. </strong>Lorem ipsum, dolor sit amet consectetur
            adipisicing elit. Maiores impedit perferendis suscipit eaque, iste dolor cupiditate blanditiis ratione.</p>
          <p class="text-black mb-8"><strong><img
                src="https://static.vecteezy.com/system/resources/thumbnails/002/360/432/small/lock-icon-free-vector.jpg"
                class="inline-block h-6 w-6 mr-2">SSL certificates. </strong>Anim aute id magna aliqua ad ad non deserunt
            sunt. Qui irure qui lorem cupidatat commodo.</p>
          <p class="text-black"><strong><img src="https://cdn-icons-png.flaticon.com/512/149/149206.png"
                class="inline-block h-6 w-6 mr-2">Database backups. </strong>Ac tincidunt sapien vehicula erat auctor
            pellentesque rhoncus. Et magna sit morbi lobortis..</p>
        </div>
      </section>
      <slot></slot>
      <section class="bg-cover bg-center rounded-l-lg h-80 sm:h-auto"
        style="background-image: url('https://tailwindui.com/img/component-images/dark-project-app-screenshot.png');">
      </section>
    </div>
  </main>
</template>
<script setup>
defineProps({
  title: String
})
</script>

<style scoped>
.btn {
  padding: 1rem;
}</style>