<script setup lang="ts">
import Test from './components/Test.vue';
import Top from './components/Top.vue'
</script>

<template>
    <div class="body">
        <Top></Top>
    </div>
</template>

<style scoped lang="scss">
.body {
    // start with mobile size
    width: 375px;
    height: 1065px;

    background: var(--white);

    margin: auto;
    padding: 24px 24px 63px 24px;
}

.--dark .body {
    background: var(--b-1);
}
</style>
