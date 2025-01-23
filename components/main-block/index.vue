<script lang="ts" setup>
defineProps({
  text: {
    type: String,
    default: 0,
  },
  bg: {
    type: String,
    default: "transparent",
  },
});
</script>

<template>
  <div :class="bg" class="main-block">
    {{ text }}
  </div>
</template>

<style lang="scss">
.main-block {
  @apply flex justify-center items-center;
  @apply h-screen;
  @apply text-white text-5xl font-bold;
}
</style>
