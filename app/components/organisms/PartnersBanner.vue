<template>
  <div class="partners-banner">
    <img src="/huh.jpg" alt="Logos des partenaires : Huh.." class="partners-banner__image" />
    <img src="/pinch.jpg" alt="Logos des partenaires : Noooon.." class="partners-banner__image" />
    <img src="/sip.jpg" alt="Logos des partenaires : Boire.." class="partners-banner__image" />
    <img src="/kneel.jpg" alt="Logos des partenaires : A genoux.." class="partners-banner__image" />
  </div>
</template>

<style scoped>
.partners-banner {
  padding: var(--spacing-xxl) 0;
  display: flex;
  align-items: center;
  justify-content: center;
  border-top: 1px solid var(--color-border);
}

.partners-banner__image {
  max-width: 600px;
  opacity: 0.5;
}
</style>