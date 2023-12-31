<template>
    <div id="sidebar">
        <div class="header">
            <img :src="logo" alt="">
            <h1>WordPilot</h1>
        </div>
        <ul>
            <li :key="index" v-for="(page, index) of pages" :class="`${page.name == 'Projects' ? 'active' : ''}`"><component :is="page.component" :key="index"></component> {{ page.name }}</li>
        </ul>
    </div>
</template>
<script setup>
    import logo from "@/assets/images/icon/Union.svg"
    import DashboardIcon from "@/components/icons/DashboardIcon.vue"
    import DocumentIcon from "@/components/icons/DocumentIcon.vue"
    import LogoutIcon from "@/components/icons/LogoutIcon.vue"
    import SchedulerIcon from "@/components/icons/SchedulerIcon.vue"
    import ContentWizardIcon from "@/components/icons/ContentWizardIcon.vue"
    import ProjectIcon from "@/components/icons/ProjectIcon.vue"
    const pages = [{name: "Dashboard", component: DashboardIcon}, {name: "Projects", component: ProjectIcon}, {name: "Scheduler", component: SchedulerIcon}, {name: "Content Wizard", component: ContentWizardIcon}, {name: "Documents", component: DocumentIcon}, {name: "Log Out", component: LogoutIcon}]
</script>
<style scoped lang="less">
    @import "../css/less/style.less";
    #sidebar{
        width: @sidebar;
        position: fixed;
        top: 0;
        left: 0;
        bottom: 0;
        z-index: 50;
        background: @primary;
        padding: 30px 27px;

        .header{
            display: flex;
            align-items: center;
            padding: 15px 15px 40px 15px;
            border-bottom: 1px solid @border-light;
            height: fit-content;
            margin-bottom: 30px;
            gap: 10px;
            h1{
                color: #fff;
                font-size: 27px;
            }

        }
        ul{
            display: flex;
            flex-direction: column;
            gap: 8px;

            li{
                list-style: none;
                padding: 12px;
                color: @secondary;
                font-weight: 700;
                border-radius: 4px;
                display: flex;
                align-items: center;
                gap: 10px;
                &:hover, &.active{
                    background-color: @primary-blue;
                    color: white;
                }
            }
        }
    }
</style>