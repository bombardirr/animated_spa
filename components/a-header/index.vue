<script lang="ts" setup>
const links = {
  pageZero: "/",
  pageOne: "/pageOne",
  pageTwo: "/pageTwo",
  pageThree: "/pageThree",
  pageFour: "/pageFour",
};
</script>

<template>
  <div class="header">
    <nav>
      <ul>
        <li><NuxtLink :to="links.pageZero">HOME</NuxtLink></li>
        <li><NuxtLink :to="links.pageOne">PAGE 1</NuxtLink></li>
        <li><NuxtLink :to="links.pageTwo">PAGE 2</NuxtLink></li>
        <li><NuxtLink :to="links.pageThree">PAGE 3</NuxtLink></li>
        <li><NuxtLink :to="links.pageFour">PAGE 4</NuxtLink></li>
      </ul>
    </nav>
  </div>
</template>

<style lang="scss">
.header {
  @apply fixed left-0 right-0 top-0 z-30;
  @apply w-screen;
  @apply bg-white;

  nav {
    ul {
      @apply flex justify-evenly items-center;
    }
  }
}
</style>
