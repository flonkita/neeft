<template>
  <div class="home-layout">
    <OrganismsTheHeader />
    
    <main class="home-layout__main">
      <div class="home-layout__content">
        <OrganismsHeroSection />
      </div>
    </main>
    
    <OrganismsPartnersBanner />
  </div>
</template>

<style scoped>
.home-layout {
  display: flex;
  flex-direction: column;
  min-height: 100vh;
}

.home-layout__main {
  flex-grow: 1;
  padding-top: calc(var(--spacing-hero) + 80px);
  padding-bottom: var(--spacing-xxl);
}

.home-layout__content {
  max-width: 1400px;
  margin: 0 auto;
  padding: 0 var(--spacing-l);
}
</style>