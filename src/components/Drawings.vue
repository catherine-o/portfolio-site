<template>
    <div class='drawings'>
        <h2>DRAWINGS</h2>
        <p>Coming soon...</p>
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
    .arrows {
        width: 25px;
        opacity: 60%;
        position: relative;
        left: 46%;
        margin-top: 35%;
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