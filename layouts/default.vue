<template>
  <div class="default-layout">
    <a-header />
    <div>
      <main>
        <slot />
      </main>
    </div>
    <a-footer />
  </div>
</template>

<style lang="scss">
.default-layout {
  @apply relative flex flex-col;
}
</style>
