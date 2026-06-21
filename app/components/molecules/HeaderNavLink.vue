<script setup lang="ts">
defineProps({
  to: {
    type: String,
    required: true
  }
})
</script>

<template>
  <NuxtLink :to="to" class="nav-link">
    <slot />
    <span class="nav-link__underline"></span>
  </NuxtLink>
</template>

<style scoped>
.nav-link {
  display: inline-flex;
  flex-direction: column;
  color: var(--color-text-primary);
  font-size: var(--font-size-nav);
  font-weight: var(--font-weight-medium);
  transition: var(--transition);
}

.nav-link:hover {
  color: var(--color-primary);
}

.nav-link__underline {
  height: 2px;
  width: 0;
  background-color: var(--color-primary);
  transition: var(--transition);
  margin-top: 2px;
}

.nav-link:hover .nav-link__underline {
  width: 100%;
}
</style>