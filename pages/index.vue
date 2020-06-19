<template>
  <div>
    <h1>polyfill</h1>
    <ul>
      <li><nuxt-link to="/page1">polyfill - Array.prototype.includes</nuxt-link></li>
      <li><nuxt-link to="/page2">polyfill - Promise, FetchAPI in CSR</nuxt-link></li>
    </ul>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({})
</script>
