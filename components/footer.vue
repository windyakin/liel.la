<template>
  <footer
    :class="$style.footer"
    :style="{ height: height, lineHeight: height }"
  >
    <b-container>
      <span class="text-muted">
        Produced by windyakin
        <a href="https://twitter.com/MITLicense">@MITLicense</a>
      </span>
    </b-container>
  </footer>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
  props: {
    height: {
      type: String,
      required: true,
    },
  },
})
</script>

<style module>
.footer {
  position: absolute;
  bottom: 0;
  width: 100%;
  background-color: #f5f5f5;
  text-align: right;
}
</style>
