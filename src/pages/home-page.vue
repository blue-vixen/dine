<template>
    <section class="home-page">
        <main-hero />
        <second-hero />
        <highlights />
        <cards />
        <call-to-action />
        <app-footer />
    </section>
</template>

<script>
import mainHero from "../components/main-hero.vue";
import secondHero from "../components/second-hero.vue";
import highlights from "../components/highlights.vue";
import cards from "../components/cards.vue";
import callToAction from "../components/call-to-action.vue";
import appFooter from "../components/app-footer.vue";
export default {
    components: {
        mainHero,
        secondHero,
        highlights,
        cards,
        callToAction,
        appFooter,
    },
};
</script>

<style>
</style>
