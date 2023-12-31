<template>
    <div class="flex gap-5 items-center">
        <input :class="$style.check" type="checkbox" name="" :id="$style.check">
        <label :class="$style['label']" :for="$style.check">{{ props.title }}</label>
    </div>
</template>
<style module>
    .check{
        color: purple;
    }
    label{
        font-size: 15px;
    }
</style>

<script setup>
const props = defineProps({
    title: String
})
</script>