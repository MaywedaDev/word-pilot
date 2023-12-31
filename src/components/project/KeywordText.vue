<template>
    <div id="keywordtext" class="w-full">
        <div class="flex justify-between">
            <div class="header">
                <h6>Keyword to Include in the text</h6>
                <p>If you do not provide the keywords, we will automatically generate relevant keywords from the main keyword for each section and use them to generate the article.</p>
            </div>
            <button>NLP Keyword Generator</button>
        </div>
        <Card title="">
            <div id="keywords" class="flex">
                <button v-for="item of keywords" class="keyword"><span>{{ item }}</span><span class="cancel">x</span></button>
            </div>
            <input type="text" placeholder="Some keyword or phrase relevant to your blog, then press Enter or + to add">
        </Card>
    </div>
</template>
<script setup>
    import Card from '../Card.vue';

    const keywords = [
        "what do dermatologists prescribe for skin whitening?",
        "dermatologist prescribe",
        "skin whitening treatment",
        "dermatologist recommend skin whitening products",
        "skin lightening creams prescribed by dermatologists",
        "prescription medications for skin whitening",
        "professional skin whitening treatments",
        "dermatologist approved skin lightening treatments",
        "topical skin whitening prescriptions"
    ]
</script>
<style scoped lang="less">
@import "../../css/less/variables.less";
#keywordtext{
    > * {
        margin-bottom: 20px;
    }
    .header{
        h6{
            font-size: 16px
        }   
        p{
            font-size: 15px;
            color: #6B6B6B;
        }
    }
    #keywords{
        flex-wrap: wrap;
        margin-top: 0;
        gap: 10px;
        .keyword{
            font-size: 13px;
            display: flex;
            gap: 30px;
            align-items: center;
            padding: 8px;
            border-radius: 4px;
            color: white;
        }
    }
    span{
        display: inline-block;
        &.cancel{
            color: #6B6B6B;
        }
    }
    button{
        padding: 15px 35px;
        font-size: 14px;
    }
    input{
        padding: 12px;
        border: none;
        outline: none;
        width: 100%;
    }
}
</style>
