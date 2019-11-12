<template>
    <div class='writings'>
        <h2>WRITINGS</h2>
        <div class='post-grid'>
            <div class='post' @click='openRailsAuthPost'>
                <img class='post-img' src='../assets/blog/authlock.jpeg'>
                <h3>Auth with JSON Web Tokens & BCrypt (Part I: Rails)</h3>
                <p>
                    In this article, we will be walking through 
                    how to set up user auth in your backend by 
                    creating JWTs for storing…
                </p>
                <h4>Oct 6, 2019</h4>
            </div>
            <div class='post' @click='openMusicPost'>
                <img class='post-img' src='../assets/blog/music.png'>
                <h3>Learning to Code is like Learning to Play an Instrument</h3>
                <p>
                    After having some time to dive into different 
                    programming languages and building a few 
                    programs, I’ve noticed...
                </p>
                <h4>Sep 16, 2019</h4>
            </div>
            <div class='post' @click='openBashPost'>
                <img class='post-img' src='../assets/blog/bash.png'>
                <h3>When the BASH Ain’t Got *Flash* — Beautify the CLI</h3>
                <p>
                    By default, the BASH terminal is not very 
                    pretty. Sure, it can be functional and get 
                    the point across, but if you’re...
                </p>
                <h4>Aug 18, 2019</h4>
            </div>
        </div>
        <img class='arrows' @click='scrollToTop' src='../assets/icons/uparrows.svg' alt='Page Up'>
    </div>
</template>

<script>
export default {
    methods: {
        openRailsAuthPost() {
            window.open('https://medium.com/swlh/auth-with-json-web-tokens-bcrypt-part-i-rails-3afd71751ea', '_blank')
        },
        openMusicPost() {
            window.open('https://medium.com/swlh/learning-to-code-is-like-learning-to-play-an-instrument-61517299fe3f', '_blank')
        },
        openBashPost() {
            window.open('https://medium.com/@oharacatherine/when-the-bash-aint-got-flash-beautify-the-cli-5f318325a86', '_blank')
        },
        scrollToTop() {
            window.scrollTo({ top: 0, behavior: 'smooth' })
        }
    }
}
</script>

<style lang="scss">
.writings {
    background-image: url('../assets/backgrounds/flowers-mobile.jpeg');
    background-position: center;
    background-attachment: fixed;
    background-repeat: no-repeat;
    width: 100%;
    padding-top: 5%;
    @media screen and (min-width: 820px) {
        background-image: url('../assets/backgrounds/flowers-desktop.jpeg');
    }
    @media screen and (min-width: 1420px) {
        padding: 2% 0;
        height: 85vh;
    }
    h2 {
        background-color: white;
        width: 200px;
        padding: 15px 10px;
        margin: auto;
    }
    .post-grid {
        margin: 5% auto;
        background-color: white;
        padding-bottom: 5%;
        @media screen and (min-width: 700px) {
            width: 70%;
        }
        @media screen and (min-width: 1430px) {
            width: 80%;
            height: 425px;
            margin: 3% auto;
            padding: 10px 20px;
            display: flex;
            flex-flow: row wrap;
            justify-content: space-evenly;
        }
        .post {
            padding: 20px;
            @media screen and (min-width: 700px) {
            padding: 50px 100px 0 100px;
            }
            @media screen and (min-width: 1430px) {
            padding: 30px;
            margin: auto;
            max-width: 320px;
            }
            .post-img {
                width: 90%;
                @media screen and (min-width: 700px) {
                    width: 320px;
                }
            }
            h4 {
                opacity: 0.6;
                font-size: 15px;
            }
        }
        .post:hover h3 {
            color: rgb(81, 141, 121);
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
    }
}
</style>