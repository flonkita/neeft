<template>
  <section class="hero-section">
    <div class="hero-section__content">
      <span class="hero-section__category">Joueurs, staffs et équipes Esports</span>
      
      <h1 class="hero-section__title">La porte d'entrée entre les talents et les équipes qui recrutent</h1>
      
      <p class="hero-section__description">NEEFT centralise le recrutement esport pour aider les bons profils à rencontrer les bonnes structures.</p>
      
      <div class="hero-section__actions">
        <AtomsAppButton variant="primary">Créé ton profil gratuitement</AtomsAppButton>
        <AtomsAppButton variant="secondary">Voir les talents</AtomsAppButton>
      </div>
    </div>
    
    <OrganismsHeroVideoPlayer />
  </section>
</template>

<style scoped>
/* --- Styles de l'Organisme Hero --- */
.hero-section {
  display: flex;
  align-items: center;
  justify-content: space-between;
  gap: var(--spacing-xxl);
}

.hero-section__content {
  max-width: 600px;
}

/* C'est ICI que commence la "ligne d'intro" orange */
.hero-section__category {
  display: inline-block;
  font-size: 13px;
  color: var(--color-primary); /* Orange */
  margin-bottom: var(--spacing-m);
}

.hero-section__title {
  font-family: var(--font-family);
  font-size: var(--font-size-hero-title);
  font-weight: var(--font-weight-bold);
  color: var(--color-text-primary);
  line-height: 1.2;
  margin-bottom: var(--spacing-l);
}

.hero-section__description {
  font-size: var(--font-size-hero-subtitle);
  color: var(--color-text-muted);
  max-width: 500px;
  margin-bottom: var(--spacing-xxl);
}

.hero-section__actions {
  display: flex;
  gap: var(--spacing-m);
}
</style>