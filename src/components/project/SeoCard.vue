<template>
    <Card title="SEO">
        <div id="seocard" class="w-full">
            <div class="grid">
                <div class="text-field">
                    <label>SEO Score</label>
                    <select>
                        <option value="">0 - 20%</option>
                    </select>
                </div>
                <div class="text-field">
                    <label>Keyword Density</label>
                    <select>
                        <option value="">10 times</option>
                    </select>
                </div>
                <div class="text-field">
                    <label>Tags</label>
                    <select>
                        <option value="">None</option>
                    </select>
                </div>
            </div>
            <Checkbox title="Use the main keyword to write and insert a meta description in the post. Also relevant keyword will be picked up and added to the meta description."/>
        </div>
    </Card>
</template>
<script setup>
    import Card from '../Card.vue';
    import Checkbox from '../Checkbox.vue';
</script>
<style scoped lang="less">
    #seocard{
        > :not(:last-child){
            margin-bottom: 20px;
        }
    }
    .grid{
        display: grid;
        max-width: 810px;
        grid-template-columns: repeat(3, 1fr);
        gap: 40px;
    }
</style>