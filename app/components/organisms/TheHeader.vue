<template>
  <header class="header">
    <div class="header__container">
      <AtomsAppLogo />
      <nav class="header__nav">
        <ul class="header__nav-list">
          <li class="header__nav-item">
            <MoleculesHeaderNavLink to="/joueurs">Joueurs</MoleculesHeaderNavLink>
          </li>
          <li class="header__nav-item">
            <MoleculesHeaderNavLink to="/equipes">Équipes</MoleculesHeaderNavLink>
          </li>
          <li class="header__nav-item">
            <MoleculesHeaderNavLink to="/recrutement">Recrutement</MoleculesHeaderNavLink>
          </li>
          <li class="header__nav-item">
            <MoleculesHeaderNavLink to="/staff">Staff</MoleculesHeaderNavLink>
          </li>
          <li class="header__nav-item">
            <MoleculesHeaderNavLink to="/carte">Carte</MoleculesHeaderNavLink>
          </li>
          <li class="header__nav-item">
            <MoleculesHeaderNavLink to="/tarification">Tarification</MoleculesHeaderNavLink>
          </li>
        </ul>
      </nav>
      <MoleculesUserProfileButton />
    </div>
  </header>
</template>

<style scoped>
.header {
  position: fixed;
  top: 0;
  left: 0;
  right: 0;
  background-color: rgba(13, 17, 23, 0.9);
  backdrop-filter: blur(8px);
  z-index: 1000;
  border-bottom: 1px solid var(--color-border);
}

.header__container {
  max-width: 1400px;
  margin: 0 auto;
  padding: var(--spacing-s) var(--spacing-l);
  display: flex;
  align-items: center;
  justify-content: space-between;
}

.header__nav-list {
  display: flex;
  align-items: center;
  gap: var(--spacing-l);
}
</style>