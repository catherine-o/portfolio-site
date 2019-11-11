<template>
    <div class='contact'>
        <h2>CONTACT</h2>
        <div class='contact-form' @submit.prevent='submitForm'>
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
            this.validateInputs
        },
        validateInputs() {
            
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
    height: 80vh;
    padding-top: 5%;
    @media screen and (min-width: 1420px) {
        // padding-top: 5%;
        height: 85vh;
    }
    h2 {
        background-color: white;
        width: 200px;
        padding: 15px 10px;
        margin: auto;
    }
    .contact-form {
        width: 50%;
        margin: 5% auto;
        .pageclip-form {
            display: flex;
            flex-flow: column nowrap;
            input, textarea {
                font-family: 'Avenir', Helvetica, Arial, sans-serif;
                -webkit-font-smoothing: antialiased;
                -moz-osx-font-smoothing: grayscale;
                height: 35px;
                margin: 10px 0;
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
                // background-color: rgb(109, 114, 163);
                background-color: rgb(219, 163, 89);
                color: white;
                font-size: 15px;
                margin-top: 10px;
                margin-left: auto;
                border: none;
            }
        }
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