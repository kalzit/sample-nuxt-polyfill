<template>
  <div>
    <h1>polyfill</h1>
    <p>Promise, FetchAPI in CSR</p>
    <p>{{ result }}</p>
  </div>
</template>

<script lang="ts">
import { Context } from '@nuxt/types'
import Vue from 'vue'

export default Vue.extend({
  data(): { result : string } {
    return { result: '' }
  },
  async mounted(): Promise<void> {
    const res = await fetch('https://yesno.wtf/api')
    const json = await res.json()
    this.result = json;
  }
})
</script>
