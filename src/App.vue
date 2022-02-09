<template>
    <div id="app">
        <home-page />
    </div>
</template>

<script>
import homePage from "../src/pages/home-page.vue";
export default {
    name: "App",
    components: {
        homePage,
    },
};
</script>
