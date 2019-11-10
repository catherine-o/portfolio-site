<template>
    <div class='writings'>
        <h2>WRITINGS</h2>
        <div class='post-grid'>
            <div class='post'>
                <img class='post-img' src='../assets/blog/authlock.jpeg'>
                <h3>Auth with JSON Web Tokens & BCrypt (Part I: Rails)</h3>
                <p>
                    In this article, we will be walking through 
                    how to set up user auth in your backend by 
                    creating JWTs for storing…
                </p>
                <h4>Oct 6, 2019</h4>
            </div>
            <div class='post'>
                <img class='post-img' src='../assets/blog/music.png'>
                <h3>Learning to Code is like Learning to Play an Instrument</h3>
                <p>
                    After having some time to dive into different 
                    programming languages and building a few 
                    programs, I’ve noticed...
                </p>
                <h4>Sep 16, 2019</h4>
            </div>
            <div class='post'>
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
    .post-grid {
        width: 80%;
        height: 420px;
        background-color: white;
        margin: 5% auto;
        padding: 10px 20px;
        display: flex;
        justify-content: space-evenly;
        .post {
            padding: 30px;
            margin: auto;
            .post-img {
                width: 320px;
            }
            h4 {
                opacity: 60%;
            }
        }
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