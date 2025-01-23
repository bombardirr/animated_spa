<script lang="ts" setup>
const links = [
  { to: "/", title: "Home" },
  { to: "/pageOne", title: "PageOne" },
  { to: "/pageTwo", title: "PageTwo" },
  { to: "/pageThree", title: "PageThree" },
  { to: "/pageFour", title: "PageFour" },
];
</script>

<template>
  <div class="header">
    <nav>
      <ul>
        <li v-for="link of links" :key="link.title">
          <NuxtLink :to="link.to">{{ link.title }}</NuxtLink>
        </li>
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
