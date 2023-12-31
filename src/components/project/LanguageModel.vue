<template>
    <div id="model">
        <h6 class="font-bold font-col">Language Model</h6>
        <div class="grid">
            <div class="text-field">
                <label>Quality Type</label>
                <select>
                    <option value="">GPT 3.5 + GPT 3.5 Turbo 16k + GPT 4</option>
                </select>
            </div>
            <p>For optimal resalts, we use a mix of different models in cluding GPT 3.5, GPT 3.5 Turbo 16K, and GPT 4 8K ensuring the best quality.</p>
        </div>
        <div class="grid">
            <div class="text-field">
                <label>Open API Key</label>
                <select>
                    <option value="">No</option>
                </select>
            </div>
            <p>You can connect your API key if you have used up our words and still have unspent Article Generations limits.</p>
        </div>
    </div>
</template>

<style scoped lang="less">
    #model{
        h6{
            font-size: 16px
        }
        > :not(:last-child){
            margin-bottom: 20px;
        }
    }
    .grid{
        display: grid;
        grid-template-columns: 450px auto;
        max-width: 1200px;
        gap: 40px;
        align-items: end;
        p{
            color: #6B6B6B;
            font-size: 15px;
        }
    }
</style>