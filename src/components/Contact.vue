<template>
    <div class='contact'>
        <h2>CONTACT</h2>
        <div class='contact-form'>
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
.contact {
    background-image: url('../assets/plant.jpeg');
    background-position: center;
    background-attachment: fixed;
    background-repeat: no-repeat;
    width: 100%;
    padding-top: 5%;
    @media screen and (min-width: 1420px) {
        padding-top: 3%;
        height: 85vh;
    }
    h2 {
        background-color: white;
        width: 200px;
        padding: 15px 10px;
        margin: auto;
    }
    .arrows {
        background-color: white;
        padding: 5px;
        width: 25px;
        opacity: 80%;
        position: relative;
        left: 42%;
        margin: -20px 0 20px 0;
        @media screen and (min-width: 1000px) {
            left: 44%;
        }
    }
    .arrows:hover {
        opacity: 90%;;
    }
}
</style>