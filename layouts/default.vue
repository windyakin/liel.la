<template>
  <div>
    <Nuxt :class="$style.content" />
    <Footer height="4rem" :class="$style.footer" />
  </div>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({})
</script>

<style>
html {
  position: relative;
  min-height: 100vh;
}
body {
  margin-bottom: calc(8rem);
}
</style>

<style module>
.content {
  min-height: calc(100vh - 8rem);
}
.footer {
  margin-top: 4rem;
}
</style>
