<template>
    <section class="menu-highlights-container container dark">
        <section class="menu-highlights">
            <section class="section-description">
                <h2>A few highlights from our menu</h2>
                <p>We cater for all dietary requirements, but here's a glimpse at some of our diner's favourites. Our menu is revamped every season.</p>
            </section>
            <section class="highlights">
                <section class="dish-details" v-for="dish in dishes" :key="dish.id">
                    <img :src="require(`../assets/imgs/${dish.imgUrl}`)" />
                    <div class="dish-text">
                        <h3>{{ dish.name }}</h3>
                        <p>{{ dish.desc }}</p>
                    </div>
                </section>
            </section>
        </section>
    </section>
</template>

<script>
export default {
    name: "highlights",
    data() {
        return {
            dishes: [
                { id: 1, name: "Seared Salmon Fillet", desc: "Our locally sourced salmon served with a refreshing buckwheat summer salad.", imgUrl: "salmon.jpg" },
                { id: 2, name: "Rosemary Filet Mignon", desc: "Our prime beef served to your taste with a delicious choice of seasonal sides.", imgUrl: "mignon.jpg" },
                { id: 3, name: "Summer Fruit Chocolate Mousse", desc: "Creamy mousse combined with summer fruits and dark chocolate shavings.", imgUrl: "mousse.png" },
            ],
        };
    },
};
</script>

<style>
</style>