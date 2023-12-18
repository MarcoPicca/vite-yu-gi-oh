<template>
    <nav class="container-nav">
        <div class="container-logo">
            <img class="img-logo" src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcR7H9utyv-iWJavuk5HiVxA00dlZBPK2dzguwkhzNIOmLJeZwO0HdxxXCsDpCDIqyrZR3Q&usqp=CAU" alt="">
        </div>
        <h1 class="title">Yu-Gi-Oh API</h1>
    </nav>
</template>
<script>

export default {
    name: 'AppHeader',
   
}
</script>

<style lang="scss" scoped>
    @use '../styles/general.scss' as *;

    .container-nav{
        width: 100%;
        height: 80px;
        margin: 0 auto;
        display: flex;
        justify-content: center;
        align-items: center;
        background-color: white;
    }

    .container-logo{
        width: 25%;
        height: 80px;
        display: flex;
        justify-content: center;
        align-items: center;
    }

    .img-logo{
        widows: 100%;
        height: 40px;
    }

    .title{
        width: 25%;
        color: rgb(152, 50, 50);
        font-family: Verdana, Geneva, Tahoma, sans-serif;
        font-weight: bold;
        font-size: 40px;

    }
</style>
