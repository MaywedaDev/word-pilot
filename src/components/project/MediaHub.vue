<template>
    <Card title="Media Hub">
        <div id="mediahub" class="w-full">
            <div class="grid">
                <div class="text-field">
                    <label>AI Images</label>
                    <select>
                        <option value="">None</option>
                    </select>
                </div>
                <div class="text-field">
                    <label>Number of Images</label>
                    <select>
                        <option value="">3</option>
                    </select>
                </div>
                <div class="text-field">
                    <label>Image Style</label>
                    <select>
                        <option value="">None</option>
                    </select>
                </div>
                <div class="text-field">
                    <label>Image Size</label>
                    <select>
                        <option value="">1344x768 (16:9)</option>
                    </select>
                </div>
            </div>
            <Checkbox title="Include the main keyword in the first images as Alt text. Relevant keywords will be picked up and added to the rest of the images. "/>
            <div class="grid">
                <div class="text-field">
                    <label>YouTube Videos</label>
                    <select>
                        <option value="">Yes</option>
                    </select>
                </div>
                <div class="text-field">
                    <label>Number of Videos</label>
                    <select>
                        <option value="">1</option>
                    </select>
                </div>
                <div class="text-field">
                    <label>Layout Options</label>
                    <select>
                        <option value="">Distribute Evenly</option>
                    </select>
                </div>
            </div>
            <Checkbox title="All media element will be placed strictly under the headings. If disabled AI will decide and find the best placements."/>
        </div>
    </Card>
</template>
<script setup>
    import Card from '../Card.vue';
    import Checkbox from '../Checkbox.vue';
</script>
<style scoped lang="less">
    #mediahub{
        > :not(:last-child){
            margin-bottom: 20px;
        }
    }
    .grid{
        display: grid;
        max-width: 1200px;
        grid-template-columns: 20% 15% 30% auto;
        gap: 40px;
    }
</style>