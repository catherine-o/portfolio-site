<template>
    <div class='writings'>
        <h2>WRITINGS</h2>
        <div class='posts'>

        </div>
        <img class='arrows' @click='scrollToTop' src='../assets/icons/uparrows.svg' alt='Page Up'>
    </div>
</template>

<script>
export default {
    methods: {
        scrollToTop() {
            window.scrollTo({ top: 0, behavior: 'smooth' })
        }
    }
}
</script>

<style lang="scss">
.writings {
    background-image: url('../assets/flowers.jpeg');
    background-position: center;
    background-attachment: fixed;
    background-repeat: no-repeat;
    width: 100vw;
    height: 85vh;
    padding: 0;
    h2 {
        background-color: white;
        width: 200px;
        margin: auto;
    }
    .posts {
        width: 70%;
        height: 400px;
        background-color: white;
        margin: 5% auto;
    }
    .arrows {
        background-color: white;
        padding: 5px;
        width: 25px;
        opacity: 80%;
        position: relative;
        top: 70%;
        left: 40%;
    }
    .arrows:hover {
        opacity: 90%;;
    }
}
</style>