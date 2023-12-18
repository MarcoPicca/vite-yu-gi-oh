<template>
    <main class="container-main">
        <div class="container-btn-main">
            <button class="btn-main" type="button">
                <h1>btn</h1>
            </button>
        </div>
        <div class="container-cards">
            <CardList />
        </div>
    </main>
</template>

<script>
import CardList from './CardList.vue';

export default {
    name: 'AppMain',
    components: {
        CardList,
    }
}
</script>

<style lang="scss">
    
    
    .container-btn-main{
        width: 60%;
        height: 70px;
        display: flex;
        justify-content: flex-start;
    }

    .btn-main{
        width: 60px;
        height: 40px;
        margin-bottom: 2rem;
    }
    
    .container-cards{
        width: 60%;
        height: auto;
        padding: 1rem;
        display: flex;
        justify-content: space-evenly;
        flex-wrap: wrap;
        background-color: white;
    }

</style>