<template lang="">
    <section id='card' class="container">
            <article v-for="card in CardList" :key="card.data">
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
            CardList: [],
        }
    },

    components:{
        SingleCard
    },
}
</script>

<style lang="scss">

</style>