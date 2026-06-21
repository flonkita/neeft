<template>
  <div class="video-player">
    <div class="video-player__interface">
      <div class="video-player__line"></div>
      <div class="video-player__line video-player__line--active">
        <span class="video-player__dot"></span>
      </div>
      <div class="video-player__line"></div>
      
      <button class="video-player__play-button">
        <svg viewBox="0 0 24 24" width="20" height="20">
          <path d="M7 6v12l10-6z" fill="var(--color-primary)" />
        </svg>
      </button>
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
  height: 300px;
  padding: var(--spacing-l);
  display: flex;
  flex-direction: column;
  justify-content: center;
}

.video-player__interface {
  position: relative;
  height: 100%;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
}

.video-player__line {
  position: relative;
  height: 4px;
  background-color: var(--color-border);
}

.video-player__line--active {
  background-color: var(--color-primary);
}

.video-player__dot {
  position: absolute;
  top: -6px;
  left: 20%;
  width: 16px;
  height: 16px;
  background-color: var(--color-primary);
  border-radius: 50%;
  box-shadow: 0 0 10px rgba(249, 115, 22, 0.5);
}

.video-player__play-button {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  width: 60px;
  height: 60px;
  background-color: rgba(255, 255, 255, 0.1);
  border: 1px solid var(--color-primary);
  border-radius: 50%;
  cursor: pointer;
  display: flex;
  align-items: center;
  justify-content: center;
}

.video-player__play-button:hover {
  background-color: rgba(255, 255, 255, 0.2);
}
</style>