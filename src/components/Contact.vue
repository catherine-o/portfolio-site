<template>
    <div class='contact'>
        <h2>CONTACT</h2>
        <div class='contact-form' @submit='submitForm'>
            <form action="https://send.pageclip.co/UUAwZunWcLtVAisC9tlORP2sKTZ1m7VH" class="pageclip-form" method="post">
                <!-- Make sure inputs have a "name" attribute! -->
                <input type="text" name="name" placeholder="Your name" />
                <input type="email" name="email" value="email@example.com" />
                <textarea type="text" name="message" placeholder="Send me a message" />
                <button type="submit" class="pageclip-form__submit">
                    <span>Send</span>
                </button>
            </form>
        </div>
        <img class='arrows' @click='scrollToTop' src='../assets/icons/uparrows.svg' alt='Page Up'>
    </div>
</template>

<script>
export default {
    methods: {
        scrollToTop() {
            window.scrollTo({ top: 0, behavior: 'smooth' })
        },
        submitForm() {
            alert('Message sent!')
        }
    }
}
</script>

<style lang="scss">
.contact {
    background-image: url('../assets/backgrounds/plant-mobile.jpeg');
    background-position: center;
    background-attachment: scroll;
    background-repeat: no-repeat;
    width: 100%;
    height: 85vh;
    padding-top: 5%;
    -webkit-background-size: cover;
    -moz-background-size: cover;
    -o-background-size: cover;
    background-size: cover;
    z-index: -5;
    @media screen and (min-width: 820px) {
        background-image: url('../assets/backgrounds/plant-desktop.jpeg');
        background-attachment: fixed;
    }
    @media screen and (min-width: 1420px) {
        height: 85vh;
    }
    @media screen and (min-height: 1000px) {
        padding: 200px 0 0 0;
        height: 88vh;
    }
    @media screen and (max-height: 420px) {
        padding: 200px 0 0 0;
        height: 160vh;
    }
    h2 {
        background-color: white;
        width: 200px;
        padding: 15px 10px;
        margin: auto;
    }
    .contact-form {
            margin: 5% auto;
        @media screen and (min-width: 500px) {
            width: 80%;
        }
        @media screen and (min-width: 700px) {
            width: 70%;
        }
        @media screen and (min-width: 900px) {
            width: 60%;
        }
        @media screen and (min-width: 1150px) {
            width: 50%;
        }
        .pageclip-form {
            display: flex;
            flex-flow: column nowrap;
            input, textarea {
                font-family: 'Avenir', Helvetica, Arial, sans-serif;
                -webkit-font-smoothing: antialiased;
                -moz-osx-font-smoothing: grayscale;
                height: 35px;
                margin: 10px 15px;
                border: none;
                font-size: 15px;
                padding: 5px 15px;
            }
            textarea {
                height: 100px;
                padding: 15px;
            }
            .pageclip-form__submit {
                font-family: 'Avenir', Helvetica, Arial, sans-serif;
                -webkit-font-smoothing: antialiased;
                -moz-osx-font-smoothing: grayscale;
                width: 180px;
                height: 40px;
                background-color: rgb(219, 163, 89);
                color: white;
                font-size: 15px;
                margin: 10px 15px 0 auto;
                border: none;
            }
            .pageclip-form__submit:hover {
                background-color: rgb(224, 199, 165);
                cursor: pointer;
            }
        }
    }
    .arrows {
        background-color: white;
        border-radius: 5px;
        padding: 5px;
        width: 25px;
        opacity: 0.8;
        position: relative;
        left: 42%;
        margin: -5px 0 20px 0;
        @media screen and (min-width: 1000px) {
            left: 44%;
        }
        @media screen and (min-height: 1000px) {
            left: 40%;
        }
    }
    .arrows:hover {
        opacity: 0.9;
        cursor: pointer;
    }
}
</style>