<template>
    <el-dropdown>
        <el-icon style="margin-right: 15px"><setting /></el-icon>
        <template #dropdown>
            <el-dropdown-menu>
                <el-dropdown-item>View</el-dropdown-item>
                <el-dropdown-item>Add</el-dropdown-item>
                <el-dropdown-item>Delete</el-dropdown-item>
            </el-dropdown-menu>
        </template>
    </el-dropdown>
    <span>Tom</span>
</template>

<script lang="ts">
import { defineComponent, ref } from "vue";
import { Setting } from "@element-plus/icons";
export default defineComponent({
    components: {
        Setting,
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
