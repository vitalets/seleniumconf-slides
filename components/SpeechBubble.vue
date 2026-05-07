<template>
  <div class="speech-bubble-row">
    <img src="/avatar_1.png" alt="avatar" class="speech-avatar" />
    <div class="speech-bubble">
      <slot />
    </div>
  </div>
</template>

<style scoped>
.speech-bubble-row {
  display: flex;
  align-items: flex-end;
  margin-top: 1.5rem;
}

.speech-avatar {
  width: 5rem;
  height: 5rem;
  border-radius: 50%;
  flex-shrink: 0;
}

.speech-bubble {
  position: relative;
  margin-left: 1rem;
  background: #fffde7;
  border: 2.5px solid #17212b;
  border-radius: 1.4rem;
  padding: 0.6rem 1.2rem;
  flex: 1;
  font-size: 1.15rem;
  color: #17212b;
}

/* Tail: rotated square with only left+bottom borders, bubble's left border hides the open sides */
.speech-bubble::before {
  content: '';
  position: absolute;
  left: -10px;
  bottom: 18px;
  width: 16px;
  height: 16px;
  background: #fffde7;
  border-left: 2.5px solid #17212b;
  border-bottom: 2.5px solid #17212b;
  transform: rotate(45deg);
}
</style>
