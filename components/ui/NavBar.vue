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
      :class="/^\/blog/.test($route.path) ? 'isparent' : ''"
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
      :class="/^\/nuxt-vue/.test($route.path) ? 'isparent' : ''"
      >NUXT VUE</NuxtLink
    >
  </nav>
</template>

<script setup>
  
</script>

<style scoped>
.router-link-exact-active,
.router-link-active,
.isparent {
  @apply bg-slate-300 cursor-default;
}
</style>
