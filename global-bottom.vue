<template>
  <footer v-if="$nav.currentLayout !== 'cover'" class="slide-counter">
    {{ $nav.currentPage }} / {{ $nav.total }}
  </footer>
</template>
