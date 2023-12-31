<template>
    <div id="nav">
        <div id="navbar" class="w-full flex items-center p-md bg-white">
            <div>
                <img :src="hamburger" alt="">
            </div>
            <div class="input-group">
                <input type="text" placeholder="My Workspace">
                <button><img :src="arrowDown" alt=""></button>
            </div>
            <div class="input-group">
                <input type="text" placeholder="Search here">
                <button>Search <img :src="search" alt=""></button>
            </div>
            <img :src="notifs_none" alt="">
            <img :src="info_outline" alt="">
            <div class="flex gap-10">
                <img :src="user" class="radius-md" alt="">
                <div class="text-md">
                    <p class="font-bold">Welcome Grace</p>
                    <p class="font-light">Admin</p>
                </div>
            </div>
        </div>
        <div class="page-header flex gap-10 items-center">
                <button><img :src="backArrow"></button>
                <h5 class="font-bold">Write</h5>
        </div>
    </div>
</template>
<script setup>
    import {hamburger, arrowDown, search, notifs_none, info_outline, user, backArrow} from "@/assets/images"
</script>
<style scoped lang="less">
    @import "../css/less/style.less"; 

    #nav{
        position: fixed;
        left: 300px;
        right: 30px;
        top: 0;
        padding: 30px 0;
        background-color: @bg-col;
        z-index: 50;
    }
    .page-header{
        margin-top: 30px;
        h5{
            color: #384D67;
            font-size: 22px;
        }
        button{
            padding: 6px 12px;
        }
    }
    #navbar{
        border-radius: 5px;
        gap: 30px;

        .input-group{
            width: 300px;
            &:nth-of-type(2){
                width: 260px;
            }
            &:nth-of-type(3){
                margin-left: auto;
                button{
                    gap: 6px;
                    padding-left: 12px;
                    padding-right: 12px;
                }
            }
        }
    }
</style>
