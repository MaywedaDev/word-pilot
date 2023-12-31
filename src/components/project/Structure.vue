<template>
    <div id="structure">
        <h6 class="font-bold font-col">Structure</h6>
        <div class="grid">
            <div class="text-field">
                <label>Conclusion</label>
                <select>
                    <option value="">Yes</option>
                </select>
            </div>
            <div class="text-field">
                <label>Tables</label>
                <select>
                    <option value="">Yes</option>
                </select>
            </div>
            <div class="text-field">
                <label>H3</label>
                <select>
                    <option value="">Yes</option>
                </select>
            </div>
            <div class="text-field">
                <label>List</label>
                <select>
                    <option value="">Yes</option>
                </select>
            </div>
            <div class="text-field">
                <label>Italics</label>
                <select>
                    <option value="">Yes</option>
                </select>
            </div>
            <div class="text-field">
                <label>Quotes</label>
                <select>
                    <option value="">Yes</option>
                </select>
            </div>
        </div>
        <div class="grid">
            <div class="text-field">
                <label>Key Takeaways</label>
                <select>
                    <option value="">Yes</option>
                </select>
            </div>
            <div class="text-field">
                <label>FAQs</label>
                <select>
                    <option value="">Yes</option>
                </select>
            </div>
            <div class="text-field">
                <label>Bold</label>
                <select>
                    <option value="">Yes</option>
                </select>
            </div>
        </div>
    </div>
</template>
<style scoped lang="less">
    #structure{
        h6{
            font-size: 16px
        }
        > :not(:last-child){
            margin-bottom: 20px;
        }
    }
    .grid{
        display: grid;
        grid-template-columns: repeat(6, 1fr);
        gap: 40px;
    }
</style>