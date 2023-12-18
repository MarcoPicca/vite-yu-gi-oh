<template lang="">
        <img :src="card.card_images.image_url_small" class="card" alt="">
        <!-- <h2>{{ card.data.data[i].name }}</h2> -->
</template>
<script>
export default {
    name: 'SingleCard',
    props:{
        card: {
            type: Object,
            required: true
        }
    },
}
</script>
<style lang="scss">
    .card{
        height: 300px;
        width: calc( 100% / 5 );
    }
</style>