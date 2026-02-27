<script setup lang="ts">
import KpiCard from '@/components/ui/KpiCard.vue'

interface KpiItem {
    label: string
    value: string
}

const kpis: KpiItem[] = [
    { label: 'Total Revenue', value: '$24,500' },
    { label: 'Users', value: '1,240' },
    { label: 'Orders', value: '320' },
    { label: 'Conversion Rate', value: '3.2%' },
]
</script>

<template>
    <section>
        <KpiCard v-for="kpi in kpis" :key="kpi.label" :label="kpi.label" :value="kpi.value" />
    </section>
</template>