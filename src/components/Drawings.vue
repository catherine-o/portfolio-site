<template>
    <div class='drawings'>
        <h2>DRAWINGS</h2>
        <div class='drawing-grid'>
            <img class='drawing-img' src='../assets/drawings/skulldrawing.jpg' alt='skull drawing'>
            <img class='drawing-img' src='../assets/drawings/echeveria.jpg' alt='skull drawing'>
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
    height: 73vh;
    .drawing-grid {
        display: flex;
        align-items: center;
        justify-content: space-evenly;
        padding-top: 20px;
        .drawing-img {
            width: 300px;
            border: 25px solid black;
        }
    }
    .arrows {
        width: 25px;
        opacity: 60%;
        position: relative;
        left: 46%;
        margin-top: 2%;
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