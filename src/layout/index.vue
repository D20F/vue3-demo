<template>
    <el-container style="height: 100vh; border: 1px solid #eee">
        <SideBar />

        <el-container>
            <el-header style="text-align: right; font-size: 12px">
                <Header />
            </el-header>
            <el-main>
                <router-view />
            </el-main>
        </el-container>
    </el-container>
</template>

<script lang="ts">
import { defineComponent, ref } from "vue";
import SideBar from "./SideBar/index.vue";
import Header from "./Header/index.vue";
export default defineComponent({
    components: {
        SideBar,
        Header,
    },
    setup() {
        ref(0);
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
