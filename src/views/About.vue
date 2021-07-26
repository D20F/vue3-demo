<template>
    <div class="about">
        <h1>This is an about page</h1>
        <h1>骨架屏demo实验</h1>
        <!-- <FacebookLoader
            viewBox="0 0 476 124"
            primaryColor="#f3f3f3"
            secondaryColor="#cccccc"
        >
        </FacebookLoader>
        <CodeLoader
            viewBox="0 0 476 124"
            primaryColor="#f3f3f3"
            secondaryColor="#cccccc"
        >
        </CodeLoader>
        <BulletListLoader
            viewBox="0 0 476 124"
            primaryColor="#f3f3f3"
            secondaryColor="#cccccc"
        >
        </BulletListLoader>
        <InstagramLoader
            viewBox="0 0 476 124"
            primaryColor="#f3f3f3"
            secondaryColor="#cccccc"
        >
        </InstagramLoader>
        <ListLoader
            viewBox="0 0 476 124"
            primaryColor="#f3f3f3"
            secondaryColor="#cccccc"
        >
        </ListLoader> -->
        <content-loader
            viewBox="0 0 476 124"
            primaryColor="#f3f3f3"
            secondaryColor="#cccccc"
        >
            <rect x="48" y="8" rx="3" ry="3" width="88" height="6" />
            <rect x="48" y="26" rx="3" ry="3" width="52" height="6" />
            <rect x="0" y="56" rx="3" ry="3" width="410" height="6" />
            <rect x="0" y="72" rx="3" ry="3" width="380" height="6" />
            <rect x="0" y="88" rx="3" ry="3" width="178" height="6" />
            <circle cx="20" cy="20" r="20" />
        </content-loader>

        <content-loader
            :width="256"
            :height="221"
            primaryColor="#41B883"
            secondaryColor="#349368"
        >
            <path
                d="M204.8 0H256L128 220.8 0 0h97.92L128 51.2 157.44 0h47.36z"
            />
            <path d="M0 0l128 220.8L256 0h-51.2L128 132.48 50.56 0H0z" />
            <path
                d="M50.56 0L128 133.12 204.8 0h-47.36L128 51.2 97.92 0H50.56z"
            />
        </content-loader>
    </div>
</template>
<script lang="ts">
import { Options, Vue } from "vue-class-component";
import {
    ContentLoader,
    FacebookLoader,
    CodeLoader,
    BulletListLoader,
    InstagramLoader,
    ListLoader,
} from "vue-content-loader";

@Options({
    components: {
        ContentLoader,
        FacebookLoader,
        CodeLoader,
        BulletListLoader,
        InstagramLoader,
        ListLoader,
    },
})
export default class About extends Vue {}
</script>
