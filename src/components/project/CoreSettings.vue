<template>
    <div>
        <h6 class="font-bold font-col">Core Settings</h6>
        <div id="settings" class="flex">
            <div class="flex flex-col field-1">
                <div class="text-field">
                    <label>Language</label>
                    <select>
                        <option value="">English (US)</option>
                    </select>
                </div>
                <div class="text-field">
                    <label>Tone of Voice</label>
                    <select>
                        <option value="">Friendly</option>
                    </select>
                </div>
                <div class="text-field">
                    <label>Point of view</label>
                    <select>
                        <option value="">None</option>
                    </select>
                </div>
                <div class="text-field">
                    <label>Target Country</label>
                    <select>
                        <option value="">None</option>
                    </select>
                </div>
            </div>
            <div class="field-2">
                <div class="flex gap-10 items-end">
                    <div class="text-field">
                        <label>Article Size</label>
                        <select>
                            <option value="">X-Small</option>
                        </select>
                    </div>  
                    <div class="desc radius-md w-full">
                        <span>2400-3600 words, 9-12 H2 headings</span>
                    </div>
                </div>
                <p>
                    The X-Small article offers short articles or news, ideal for quick updates and capturing immediate interest, ensuring your content remains fresh and timely in the eyes of your audiences.
                </p>
                <div class="flex items-center">
                    <div class="flex gap-5 items-center"><span>Detail to Include</span><img :src="info_outline" alt=""></div>
                    <div class="samples flex">
                        <span>Sample 1</span><span>Sample 2</span><span>Sample 3</span>
                    </div>
                </div>
                <Checkbox title="Intense mode: to each section, beyond just the entire article."/>
                <textarea name="" id="" cols="30" rows="5" placeholder="e.g. phone number as 267-229-6783"></textarea>
            </div>
        </div>
    </div>
</template>

<script setup>
    import { info_outline } from '@/assets/images';
    import Checkbox from '../Checkbox.vue';
</script>

<style lang="less" scoped>
    h6{
        font-size: 16px
    }
    #settings{
            margin-top: 30px;
            gap: 80px;

            .field-1{
                width: 100%;
                max-width: 450px;

                .text-field{
                    margin-bottom: 20px;
                }
            }

            .field-2{
                width: 100%;
                max-width: 500px;
                > :not(:first-child){
                    margin-top: 20px;
                }
                .desc{
                    padding: 10px;
                    background: #D3E7FF;
                    span{
                        color: #718399;
                        font-size: 13px;
                    }
                }
                .samples{
                    margin-left: 40px;
                    span{
                        &:not(:first-child){
                            border-left: 1px solid #5D93D9;
                        }
                        display: inline-block;
                        padding: 0px 8px;
                        color: #5D93D9;
                    }
                }
                p{
                    color: #6B6B6B;
                    font-size: 13px;
                }
            }
        }
</style>