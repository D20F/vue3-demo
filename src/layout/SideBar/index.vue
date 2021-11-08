<template>
    <el-aside width="200px" style="background-color: rgb(238, 241, 246)">
            <!-- :background-color="variables.menuBg"
            :text-color="variables.menuText"
            :active-text-color="variables.menuActiveText" -->
        <el-menu
        >
            <el-sub-menu index="3">
                <template #title>
                    <el-icon><setting /></el-icon>Navigator Three
                </template>
                <el-menu-item index="3-1">Option 1</el-menu-item>
                <el-menu-item index="3-2">Option 2</el-menu-item>
            </el-sub-menu>
        </el-menu>
        <el-menu>
            <el-sub-menu index="3">
                <template #title>
                    <el-icon><setting /></el-icon>Navigator Three
                </template>
                <el-menu-item index="3-1">Option 1</el-menu-item>
                <el-menu-item index="3-2">Option 2</el-menu-item>
            </el-sub-menu>
        </el-menu>
    </el-aside>
</template>

<script lang="ts">
import { defineComponent, ref } from "vue";
// import variables from "@/styles/variables.scss";
import { Menu, Setting } from "@element-plus/icons";

export default defineComponent({
    components: {
        // Message,
        Setting,
        // "icon-menu": Menu,
    },
    setup() {
        ref();
    },
    computed: {
        // variables() {
        //     return variables;
        // },
    },
});
</script>

<style>
.el-header {
    background-color: #b3c0d1;
    color: var(--el-text-color-primary);
    line-height: 60px;
}

.el-aside {
    color: var(--el-text-color-primary);
}
</style>
