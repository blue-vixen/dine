<template>
    <section class="cards-container container light">
        <section class="cards">
            <article class="card">
                <img :src="require(`../assets/imgs/${cards[0].imgUrl}`)" />
                <div class="card-text">
                    <h2>{{ cards[0].header }}</h2>
                    <p>{{ cards[0].desc }}</p>
                    <button>Book a table</button>
                    <ul class="card-nav clean-list">
                        <li>Family Gathering</li>
                        <li>Special Events</li>
                        <li>Social Events</li>
                    </ul>
                </div>
            </article>
        </section>
    </section>
</template>

<script>
export default {
    data() {
        return {
            cards: [{ id: 1, header: "Family Gathering", desc: "We love catering for entire families. So please bring everyone along for a special meal with your loved ones. We'll provide a memorable experience for all.", imgUrl: "gathering.png" }],
        };
    },
};
</script>

<style>
</style>