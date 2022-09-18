<template>
  <div>
    <Body class="bg-sky-300" />
    <Title>😄</Title>
    <NuxtLayout>
      <NuxtPage />
    </NuxtLayout>
  </div>
</template>

<script setup>
useHead({
  htmlAttrs: {
    lang: "ru",
  },
  bodyAttrs: {
    class: "bg-green-400"
  }
})
</script>
