<template>
  <nav class="flex items-center justify-start p-3 gap-4">
    <NuxtLink
      to="/"
      class="bg-slate-100 hover:bg-slate-300 leading-none pt-1 pb-1.5 px-5 rounded-3xl font-semibold text-xl text-slate-800 transition duration-150"
      >Home</NuxtLink
    >
    <NuxtLink
      to="/blog"
      class="bg-slate-100 hover:bg-slate-300 leading-none pt-1 pb-1.5 px-5 rounded-3xl font-semibold text-xl text-slate-800 transition duration-150"
      >Blog</NuxtLink
    >
    <NuxtLink
      to="/blog/about"
      class="bg-slate-100 hover:bg-slate-300 leading-none pt-1 pb-1.5 px-5 rounded-3xl font-semibold text-xl text-slate-800 transition duration-150"
      >About</NuxtLink
    >
    <NuxtLink
      to="/nuxt-vue"
      class="bg-slate-100 hover:bg-slate-300 leading-none pt-1 pb-1.5 px-5 rounded-3xl font-semibold text-xl text-slate-800 transition duration-150"
      >NUXT VUE</NuxtLink
    >
    <div>{{ /^\/blog/.test($route.path) }}</div>
    <!-- <div>{{ id }}</div> -->
  </nav>
</template>

<script setup>
// import { computed } from "vue"

const route = useRoute()
// const id = computed(() => route.value.params)

// console.log(id)

// const isparent = computed(() => {
//   return $route.path === ""
// })
</script>

<style scoped>
.router-link-exact-active,
.router-link-active,
.isparent {
  @apply bg-slate-300 cursor-default;
}
</style>
