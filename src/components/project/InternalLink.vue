<template>
    <Card title="Internal Link">
        <div id="internallink" class="w-full">
            <div class="grid">
                <div class="text-field">
                    <label>Insert Internal Link</label>
                    <select>
                        <option value="">Yes</option>
                    </select>
                </div>
                <div class="text-field">
                    <label>Number of Internal Link</label>
                    <select>
                        <option value="">5</option>
                    </select>
                </div>
                <div class="text-field">
                    <label>Post Links</label>
                    <textarea name="" id="" cols="30" rows="4" placeholder="Enter link url per line"></textarea>
                </div>
            </div>
        </div>
    </Card>
</template>
<script setup>
    import Card from '../Card.vue';
</script>
<style scoped lang="less">
    #internallink{
        > :not(:last-child){
            margin-bottom: 20px;
        }
    }
    .grid{
        display: grid;
        grid-template-columns: 20% 20% auto;
        gap: 40px;
    }
</style>