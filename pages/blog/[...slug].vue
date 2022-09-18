<template>
  <main class="prose pt-16 mx-auto max-w-prose">
    <ContentDoc>
      <template #not-found>
        <h2>Статья {{ $route.params.slug }} не найдена.</h2>
      </template>
    </ContentDoc>
  </main>
</template>
