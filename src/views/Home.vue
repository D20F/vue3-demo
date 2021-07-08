<template>
    <div class="home">
        <img alt="Vue logo" src="../assets/logo.png" />
        <HelloWorld msg="Welcome to Your Vue.js + TypeScript App">
            <template v-slot:foot>
                <h1>foot</h1>
            </template>
            <template v-slot:head="slotProps">
                <h1>head {{ slotProps.msg }}</h1>
            </template>

            完成具名插槽 解构插槽
        </HelloWorld>
    </div>
</template>

<script lang="ts">
import { Options, Vue } from "vue-class-component";
import HelloWorld from "@/components/HelloWorld.vue"; // @ is an alias to /src
// import { reactive, toRefs } from "vue";

@Options({
    components: {
        HelloWorld,
    },
})
export default class Home extends Vue {
    beforeCreate() {
        console.log("beforeCreate");
    }
    created() {
        console.log("created");
    }
    beforeMount() {
        console.log("beforeMount");
    }
    mounted() {
        console.log("mounted");
    }
    beforeUpdate() {
        console.log("beforeUpdate");
    }
    updated() {
        console.log("updated");
    }
    beforeUnmount() {
        console.log("beforeUnmount");
    }
    unmounted() {
        console.log("unmounted");
    }
    setup() {
        console.log(21);
        // const book = reactive({
        //     author: "Vue Team",
        //     year: "2020",
        //     title: "Vue 3 Guide",
        //     description: "You are reading this book right now ;)",
        //     price: "free",
        // });

        // let { author, title } = toRefs(book);

        // title.value = "Vue 3 Detailed Guide"; // 我们需要使用 .value 作为标题，现在是 ref
        // console.log(book.title); // 'Vue 3 Detailed Guide'
    }
}
</script>
