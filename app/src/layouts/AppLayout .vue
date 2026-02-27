<script setup lang="ts">
</script>

<template>
    <div class="layout">
        <Sidebar />
        <div class="content">
            <Header />
            <main>
                <router-view />
            </main>
        </div>
    </div>
</template>