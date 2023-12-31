<template>
    <side-bar></side-bar>
    <div id="page">
        <top-nav></top-nav>
        <div id="page-content">
            <slot></slot>
        </div>
    </div>
</template>

<script setup>
    import SideBar from './SideBar.vue';
    import TopNav from './TopNav.vue';
</script>

<style scoped lang="less">
    @import "../css/less/variables.less";
    #page{
        width: calc(100% - @sidebar);
        margin-left: @sidebar;
        padding: 30px;
    }
</style>