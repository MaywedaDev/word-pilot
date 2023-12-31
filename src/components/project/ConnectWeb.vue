<template>
    <div id="connectweb" class="w-full">
        <h6 class="font-bold font-col">Connect to Web</h6>
        <div class="flex">
            <div class="flex flex-col small w-full">
                <div class="flex">
                    <div class="text-field">
                        <label>Network</label>
                        <select>
                            <option value="">No</option>
                        </select>
                    </div>
                    <div class="text-field">
                        <label>Source Links</label>
                        <select>
                            <option value="">No</option>
                        </select>
                    </div>
                </div>
                <div class="text-field">
                    <label>Search Source</label>
                    <select>
                        <option value="">Real-Time Search Results</option>
                    </select>
                </div>
            </div>
            <div class="w-full big">
                <h6>Search Depth</h6>
                <p>Quickly finds from thematic sources and uses them as a factual basis for writing an article</p>
                <p>The tecnology of Realtime Search Results enables the immediate acquisition of search findings, which are then utilized for article writing</p>
            </div>
        </div>

    </div>
</template>
<style scoped lang="less">
    #connectweb{
        max-width: 1200px;
        h6{
            font-size: 16px
        }
        > :not(:last-child){
            margin-bottom: 20px;
        }

        .small{
            max-width: 450px;
        }

        .big{
            color: #6B6B6B;
            p:nth-of-type(2){
                margin-top: 20px;
                margin-bottom: 45px;
            }
        }

        .flex{
            gap: 40px;
        }
    }
</style>