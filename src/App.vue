<template>
    <layout />
</template>
<script lang="ts">
import { defineComponent } from "vue";
import layout from "./layout/index.vue";

export default defineComponent({
    components: {
        layout,
    },
});
</script>
<style lang="scss">
#app {
    font-family: Avenir, Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
    height: 100%;
}
body {
    margin: 0;
    height: 100%;
    -moz-osx-font-smoothing: grayscale;
    -webkit-font-smoothing: antialiased;
    text-rendering: optimizeLegibility;
    font-family: Helvetica Neue, Helvetica, PingFang SC, Hiragino Sans GB,
        Microsoft YaHei, Arial, sans-serif;
}

html {
    height: 100%;
    box-sizing: border-box;
}
</style>
