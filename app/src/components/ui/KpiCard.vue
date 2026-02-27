<script setup lang="ts">
const props = defineProps<{
  label: string
  value: string
}>()
</script>

<template>
  <div class="kpi-card">
    <div class="kpi-card__label">{{ props.label }}</div>
    <div class="kpi-card__value">{{ props.value }}</div>
  </div>
</template>