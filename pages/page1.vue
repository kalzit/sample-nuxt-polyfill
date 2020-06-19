<template>
  <div>
    <h1>polyfill</h1>
    <p>Array.prototype.includes</p>
    <p>{{ result }}</p>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
  data(): { result: boolean } {
    return {
      result: [1, 2, 3].includes(1)
    }
  }
})
</script>
