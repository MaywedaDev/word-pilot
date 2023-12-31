<template>
    <div class="view">
        
        <div class="card">
            <h6 class="font-bold font-col">Header Settings</h6>
            <div class="input-field">
                <div class="main">
                    <div class="labels">
                        <label>Main Keyword</label>
                        <span>61/80</span>
                    </div>
                    <input value="What do dermatologist prescribe for skin whitening?">
                </div>
                <button>Regenerate Title</button>
            </div>
            <div class="input-field">
                <div class="main">
                    <div class="labels">
                        <label>Title</label>
                        <span>66/100</span>
                    </div>
                    <input value="What do dermatologist prescribe for skin whitening? Discover Now!">
                </div>
            </div>
        </div>
        <core-settings></core-settings>
        <media-hub></media-hub>
        <seo-card></seo-card>
        <keyword-text></keyword-text>
        <Structure></Structure>
        <connect-web></connect-web>
        <div class="w-full">
            <div id="urls">
                <h6 class="text-light">URLs</h6>
                <Card title=""></Card>
            </div>
        </div>
        <internal-link></internal-link>
        <div class="w-full" id="document">
            <h6 class="text-light">Document</h6>
            <div class="flex items-end gap-20">
                <div class="text-field">
                    <label>Save to Directory</label>
                    <select>
                        <option value="">Home</option>
                    </select>
                </div>
                <button>Change</button>
            </div>
        </div>
        <Card title="Publish to Wordpress">
            <div class="flex" id="publish">
                <div class="text-field">
                    <label>Publication</label>
                    <select>
                        <option value="">No</option>
                    </select>
                </div>
                <div class="important w-full">
                    <h5>Important</h5>
                    <p>If you enable this option, all generated documents will be published on the selected site. Be careful with settings and publication date.</p>
                </div>
            </div>
        </Card>
        <language-model></language-model>
        <div class="flex" id="writeBtn">
            <button class="flex justify-center items-center gap-5"><img :src="write" alt=""><span>Write</span></button>
        </div>
    </div>
</template>
<script setup>
    import {write} from "@/assets/images"
    import CoreSettings from "@/components/project/CoreSettings.vue"
    import MediaHub from "@/components/project/MediaHub.vue";
    import SeoCard from "@/components/project/SeoCard.vue";
    import Structure from "@/components/project/Structure.vue";
    import ConnectWeb from "@/components/project/ConnectWeb.vue";
    import Card from "@/components/Card.vue";
    import InternalLink from "@/components/project/InternalLink.vue";
    import LanguageModel from "@/components/project/LanguageModel.vue";
    import KeywordText from "@/components/project/KeywordText.vue";
</script>
<style scoped lang="less">
    .view{
        padding: 20px 0;
        margin-top: 178px;

        .card{
            &:nth-of-type(2){
                padding-bottom: 50px;
            }
        }

        h6{
            font-size: 16px
        }

        #urls{
            h6{
                margin-bottom: 15pxpx;
            }
        }

        #document{
            h6{
                margin-bottom: 15px;
            }
            .text-field{
                max-width: 120px;
            }
            button{
                padding: 14px 18px;
                font-size: 12px;
            }
        }
        #publish{
            gap: 60px;
            max-width: 1200px;
            .text-field{
                max-width: 200px;
            }
            .important{
                color: #6B6B6B;
                h5{
                    margin-bottom: 12px;
                }
            }
            
        }
        #writeBtn{
            margin-top: 40px;
            button{
                margin-left: auto;
                padding: 15px;
                width: 250px;
            }
        }
    }
    .view > div:not(:first-child){
        margin-top: 30px;
    }
</style>

