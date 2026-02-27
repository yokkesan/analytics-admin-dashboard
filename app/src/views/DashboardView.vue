<script setup lang="ts">
import KpiSection from '@/components/KpiSection.vue'
import RevenueChartSection from '@/components/RevenueChartSection.vue'
import TrafficSection from '@/components/TrafficSection.vue'
import ActivityTableSection from '@/components/ActivityTableSection.vue'
</script>

<template>
    <div class="dashboard">
        <div class="dashboard__kpi">
            <KpiSection />
        </div>

        <div class="dashboard__revenue dashboard-card">
            <RevenueChartSection />
        </div>

        <div class="dashboard__traffic dashboard-card">
            <TrafficSection />
        </div>

        <div class="dashboard__activity dashboard-card">
            <ActivityTableSection />
        </div>
    </div>
</template>