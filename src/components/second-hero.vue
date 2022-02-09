<template>
    <section class="second-hero container light">
        <section v-for="section in sections" :key="section.id" class="hero-section">
            <img :src="require(`../assets/imgs/${section.imgUrl}`)" />
            <div class="hero-text">
                <h2>{{ section.header }}</h2>
                <p>{{ section.text }}</p>
            </div>
        </section>
    </section>
</template>

<script>
export default {
    data() {
        return {
            sections: [
                {
                    id: 1,
                    header: "Enjoyable place for all the family",
                    text: "Our relaxed surroundings make dining with us a great experience for everyone. We can even arrange a tour of the farm before your meal.",
                    imgUrl: "enjoyable.jpg",
                },
                {
                    id: 2,
                    header: "The most locally sourced food",
                    text: "All our ingredients come directly from our farm or local fishery. So you can be sure that you're eating the freshest, most sustainable food.",
                    imgUrl: "locally.png",
                },
            ],
        };
    },
};
</script>

<style>
</style>