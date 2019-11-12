<template>
    <div class='drawings'>
        <h2>DRAWINGS</h2>
        <div class='drawing-grid'>
            <img class='drawing-img' src='../assets/drawings/skulldrawing.jpg' alt='skull drawing'>
            <img class='drawing-img' src='../assets/drawings/durerhand.jpg' alt='skull drawing'>
            <img class='drawing-img' src='../assets/drawings/sadmandrawing.jpg' alt='skull drawing'>
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
.drawings {
    padding: 5%;
    @media screen and (min-width: 1000px) {
        height: 73vh;
    }
    @media screen and (min-height: 1000px) {
        height: 85vh;
    }
    .drawing-grid {
        display: flex;
        flex-flow: row wrap;
        align-items: center;
        justify-content: space-evenly;
        @media screen and (min-height: 1000px) {
            margin: 6% 0;
        }
        .drawing-img {
            border: 25px solid black;
            width: 70vw;
            margin: 20px 0;
            @media screen and (min-height: 1000px) {
                width: 250px;
            }
            @media screen and (min-width: 1000px) {
                width: 300px;
            }
            @media screen and (min-height: 1300px) {
                width: 380px;
            }
        }
    }
    .arrows {
        width: 25px;
        opacity: 60%;
        position: relative;
        left: 46%;
        @media screen and (min-width: 1000px) {
            left: 49%;
        }
        @media screen and (min-height: 1000px) {
            left: 45%;
        }
    }
    .arrows:hover {
        opacity: 90%;;
    }
}
</style>