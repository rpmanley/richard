<template>
  <div>
    <Welcome/>
    <Socials/>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
  name: 'Home'
})
</script>

<style lang="css">
body {  
  @apply bg-black text-white p-5;
}
</style>