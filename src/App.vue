<script>
import axios from 'axios';
import AppHeader from './components/AppHeader.vue';
import CardList from './components/CardList.vue';
import AppMain from './components/AppMain.vue';

export default {
  components:{
    AppHeader,
    AppMain,
    CardList,
  },

  data() {
    return {
      card: [],
    }
  },
  methods: {

    getCards(){
      axios.get('https://db.ygoprodeck.com/api/v7/cardinfo.php?num=20&offset=0')
      .then((response) => {
        console.log(response);
        this.cardList = response.data.data;
      })

      .catch(function (error) {
        console.error(error);
      });
    }
  },

  created() {
    this.getCards();
  },

}
</script>

<template>
  <AppHeader />
    <main>
      <AppMain />  
    </main>
</template>

<style lang="scss">
  @use './styles/general.scss' as *;

  *{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
  }

  .container-main{
      width: 100%;
      height: calc( 100vh - 80px);
      background-color: #D48F38;
      display: flex;
      flex-direction: column;
      align-items: center;
      padding: 2rem;
  }

</style>
