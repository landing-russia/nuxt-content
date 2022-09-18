<template>
  <h4 class="text-2xl text-teal-500 font-bold mt-5">NUXT VUE</h4>
  <ul class="pt-3">
    <li v-for="{ _path: slug, title } in nuxtVuePosts" :key="slug">
      <NuxtLink :to="slug">{{ title }}</NuxtLink>
    </li>
  </ul>
</template>

<script setup lang="ts">
const nuxtVuePosts = await queryContent("/nuxt-vue")
  .sort({ date: -1 }) // show latest articles first
  .where({ _partial: false, _path: { $ne: '/nuxt-vue' } }) // exclude the Partial files
  .find()
</script>

<style scoped>
.router-link-active {
  @apply cursor-default no-underline;
}
</style>
