<template>
  <div class="video-player">
    <div class="video-player__interface">
      
      <div class="video-player__lines">
        <div class="video-player__line">
          <span class="video-player__dot"></span>
        </div>
        
        <div class="video-player__line">
          <button class="video-player__play-button">
            <svg viewBox="0 0 24 24" width="18" height="18">
              <path d="M7 6v12l10-6z" fill="#000" />
            </svg>
          </button>
        </div>
        
        <div class="video-player__line"></div>
      </div>

      <div class="video-player__phone">
        <div class="video-player__phone-speaker"></div>
      </div>
      
    </div>
  </div>
</template>

<style scoped>
.video-player {
  position: relative;
  background-color: var(--color-background-video);
  border: 1px solid var(--color-border);
  border-radius: var(--border-radius-video);
  width: 500px;
  height: 320px;
  display: flex;
  align-items: center;
  justify-content: center;
  overflow: hidden; /* Garde tout bien à l'intérieur de la boîte */
}

.video-player__interface {
  position: relative;
  width: 100%;
  height: 100%;
}

/* --- Les Lignes --- */
.video-player__lines {
  position: absolute;
  top: 50%;
  left: 0;
  right: 0;
  transform: translateY(-50%);
  display: flex;
  flex-direction: column;
  gap: 45px; /* L'écart parfait entre les 3 lignes */
  padding: 0 40px;
}

.video-player__line {
  position: relative;
  height: 6px; /* Plus épaisses que les précédentes */
  background-color: var(--color-primary);
  border-radius: 3px;
  width: 100%;
}

/* --- Les Éléments Interactifs --- */
.video-player__dot {
  position: absolute;
  top: 50%;
  left: 15%; /* Positionné au quart de la ligne */
  transform: translateY(-50%);
  width: 16px;
  height: 16px;
  background-color: #fff; /* Blanc solide */
  border-radius: 50%;
  box-shadow: 0 0 12px 2px rgba(255, 255, 255, 0.8); /* Effet de brillance */
  z-index: 10;
}

.video-player__play-button {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  width: 56px;
  height: 56px;
  background-color: #fff; /* Fond blanc solide */
  border-radius: 50%;
  border: none;
  cursor: pointer;
  display: flex;
  align-items: center;
  justify-content: center;
  z-index: 10;
  box-shadow: 0 4px 15px rgba(0, 0, 0, 0.4);
  transition: transform 0.2s ease;
}

.video-player__play-button:hover {
  transform: translate(-50%, -50%) scale(1.05);
}

.video-player__play-button svg {
  margin-left: 4px; /* Centre visuellement le triangle de lecture */
}

/* --- L'illusion d'optique (Le Téléphone) --- */
.video-player__phone {
  position: absolute;
  top: 50%;
  right: 60px; /* Positionné sur la droite */
  transform: translateY(-50%);
  width: 70px;
  height: 200px;
  background-color: var(--color-background); /* Utilise le noir de fond pour masquer les lignes */
  border-radius: 12px;
  border: 1px solid var(--color-border);
  z-index: 5; /* Se place par dessus les lignes, mais sous les boutons */
  display: flex;
  justify-content: center;
}

/* Le petit détail du haut-parleur sur le téléphone */
.video-player__phone-speaker {
  margin-top: 10px;
  width: 20px;
  height: 2px;
  background-color: var(--color-border);
  border-radius: 2px;
}
</style>