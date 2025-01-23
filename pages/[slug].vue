<script lang="ts" setup>
const route = useRoute();
const page = ref(route.params.slug);
</script>

<template>
  <div class="page-slug">
    <main-block :text="`Page Slug: ${page}`" bg="bg-blue-400" />
  </div>
</template>

<style lang="scss">
.page-slug {
  @apply h-screen;
}
</style>
