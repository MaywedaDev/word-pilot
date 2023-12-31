<template>
    <div class="card">
        <h6 v-if="props.title" class="font-bold font-col">{{ props.title }}</h6>
        <slot></slot>
    </div>
</template>
<script setup>
    const props = defineProps({
        title: String
    })
</script>
<style scoped>
    h6{
        font-size: 16px;
        margin-bottom: 30px;
    }
</style>