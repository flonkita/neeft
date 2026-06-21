<template>
  <div class="app-logo">
    <svg viewBox="0 0 100 100" class="app-logo__icon" width="28" height="28">
      <defs>
        <linearGradient id="gradient" x1="0%" y1="100%" x2="100%" y2="0%">
          <stop offset="0%" style="stop-color:#8b5cf6" /> <stop offset="100%" style="stop-color:#f97316" /> </linearGradient>
      </defs>
      <path d="M50 5 L15 35 V75 L50 95 L85 75 V35 L50 5" fill="url(#gradient)" stroke="none" />
    </svg>
    <span class="app-logo__text">NEEFT</span>
  </div>
</template>

<style scoped>
.app-logo {
  display: flex;
  align-items: center;
  gap: var(--spacing-xs);
}

.app-logo__icon {
  margin-top: -2px; /* Ajustement visuel */
}

.app-logo__text {
  font-weight: var(--font-weight-bold);
  font-size: 18px;
  text-transform: uppercase;
  color: var(--color-text-primary);
  background: linear-gradient(45deg, #8b5cf6, #f97316);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
}
</style>