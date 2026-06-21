<script setup lang="ts">

const props = defineProps({
  variant: {
    type: String,
    default: 'primary'
  },
  size: {
    type: String,
    default: 'medium'
  }
})
</script>

<template>
  <button :class="[
    'app-button',
    `app-button--variant-${props.variant}`,
    `app-button--size-${props.size}`
  ]">
    <slot />
  </button>
</template>

<style scoped>
.app-button {
  display: flex;
  align-items: center;
  justify-content: center;
  gap: var(--spacing-xs);
  font-family: var(--font-family);
  font-weight: var(--font-weight-medium);
  border-radius: var(--border-radius-m);
  border: 1px solid transparent;
  cursor: pointer;
  transition: var(--transition);
}

.app-button--variant-primary {
  background-color: var(--color-primary);
  color: #FFF;
}

.app-button--variant-primary:hover {
  background-color: var(--color-primary-light);
}

.app-button--variant-secondary {
  background-color: var(--color-button-dark);
  color: var(--color-text-primary);
  border-color: var(--color-border);
}

.app-button--variant-secondary:hover {
  background-color: var(--color-button-dark-hover);
}

.app-button--size-medium {
  padding: var(--spacing-m) var(--spacing-xxl);
  font-size: var(--font-size-button);
}

.app-button--size-small {
  padding: var(--spacing-s) var(--spacing-l);
  font-size: var(--font-size-nav);
}
</style>