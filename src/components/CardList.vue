<template>
    <section id='card' class="container">
            <article v-for="card in this.cardList" :key="card.id">
                <SingleCard :card="card" />
            </article>
    </section>
</template>

<script>
import SingleCard from './SingleCard.vue';

export default {
    name: 'CardList',
    data() {
        return {
            cardList: [],
        }
    },

    components:{
        SingleCard
    },
}
</script>

<style lang="scss">

</style>