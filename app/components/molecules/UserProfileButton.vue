<template>
  <div class="user-profile">
    <button class="user-profile__action-icon">
      <svg viewBox="0 0 24 24" width="20" height="20">
        <path d="M10 2a8 8 0 0 1 6.32 12.9l4.38 4.38a1 1 0 0 1-1.41 1.41l-4.38-4.38A8 8 0 1 1 10 2zm0 2a6 6 0 1 0 0 12A6 6 0 0 0 10 4z" fill="var(--color-text-primary)" />
      </svg>
    </button>
    <button class="user-profile__action-icon user-profile__action-icon--has-notif">
      <svg viewBox="0 0 24 24" width="20" height="20">
        <path d="M12 2a2 2 0 0 1 2 2v.12a8 8 0 0 1 7 7.88v3a2 2 0 0 0 .58 1.41L23 18v1a1 1 0 0 1-1 1H2a1 1 0 0 1-1-1v-1l1.42-1.42A2 2 0 0 0 3 15v-3a8 8 0 0 1 7-7.88V4a2 2 0 0 1 2-2zm0 18a3 3 0 0 1-3-3h6a3 3 0 0 1-3 3z" fill="var(--color-text-primary)" />
      </svg>
      <span class="user-profile__notif-dot"></span>
    </button>
    <div class="user-profile__user-card">
      <span class="user-profile__username">athes</span>
      <svg viewBox="0 0 24 24" width="12" height="12">
        <path d="M7 10l5 5 5-5H7z" fill="var(--color-text-primary)" />
      </svg>
    </div>
  </div>
</template>

<style scoped>
.user-profile {
  display: flex;
  align-items: center;
  gap: var(--spacing-m);
}

.user-profile__action-icon {
  background: none;
  border: none;
  cursor: pointer;
  position: relative;
}

.user-profile__action-icon:hover {
  opacity: 0.8;
}

.user-profile__notif-dot {
  position: absolute;
  top: 0px;
  right: 1px;
  width: 8px;
  height: 8px;
  background-color: var(--color-primary);
  border-radius: 50%;
  border: 1px solid var(--color-background);
}

.user-profile__user-card {
  display: flex;
  align-items: center;
  gap: var(--spacing-xs);
  color: var(--color-text-primary);
  font-size: var(--font-size-nav);
  font-weight: var(--font-weight-medium);
}
</style>