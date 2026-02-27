<script setup lang="ts">
import { ref, watch } from 'vue'

const isDark = ref(false)

watch(isDark, (value) => {
  document.documentElement.classList.toggle('dark', value)
})
</script>

<template>
  <div>
    <button @click="isDark = !isDark" style="position: fixed; top: 20px; right: 20px;">
      Toggle Theme
    </button>

    <router-view />
  </div>
</template>