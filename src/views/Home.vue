<template>
    <div >
        <div class='home'>
            <header>
                <h1 >CATHERINE O'HARA</h1>
                <div class='icons'>
                    <a href='https://www.linkedin.com/in/catherine-o/' target='_blank'>
                        <img src='../assets/icons/linkedinlogo.svg' alt='LinkedIn'></a>
                    <a href='https://github.com/catherine-o' target='_blank'>
                        <img src='../assets/icons/githublogo.png' alt='GitHub'></a>
                    <a href='https://medium.com/@oharacatherine' target='_blank'>
                        <img src='../assets/icons/mediumlogo.svg' alt='Medium'></a>
                    <a href='https://twitter.com/catherine__oh' target='_blank'>
                        <img src='../assets/icons/twitterlogo.svg' alt='Twitter'></a>
                    <a href='https://docs.google.com/presentation/d/13KNWovJC7EkSLTLU-HEQKly9R2E4Xvr9a0UGxvnCyC8/edit?usp=sharing' target='_blank'>
                        <img src='../assets/icons/resumelogo.svg' alt='Resume'></a>
                </div>
            </header>
            <div class='sections'>
                <About />
                <Projects />
                <Writings />
                <Drawings />
                <Contact />
            </div>
        </div>
    </div>
</template>

<script>
import About from '@/components/About'
import Projects from '@/components/Projects'
import Writings from '@/components/Writings'
import Drawings from '@/components/Drawings'
import Contact from '@/components/Contact'
export default {
    components: {
        About,
        Projects,
        Writings,
        Drawings,
        Contact
    }
}
</script>

<style lang="scss">
.home {
    background-image: url('../assets/backgrounds/leaves-mobile-sm.jpeg');
    background-position: center;
    background-attachment: scroll;
    background-repeat: no-repeat;
    width: 100%;
    height: 100vh;
    -webkit-background-size: cover;
    -moz-background-size: cover;
    -o-background-size: cover;
    background-size: cover;
    z-index: -5;
    @media screen and (min-width: 820px) {
        background-image: url('../assets/backgrounds/leaves-desktop.jpeg');
        background-attachment: fixed;
    }
    @media screen and (max-height: 420px) {
       height: 150vh;
    }
    header {
        font-family: 'Montserrat', sans-serif;
        letter-spacing: 2px;
        background-color:rgb(231, 223, 216);
        position: fixed;
        padding: 14px 0;
        text-align: center;
        z-index: 3;
        font-size: 20px;
        width: 102%;
        @media screen and (min-width: 500px) {
            padding: 14px 0;
        }
        @media screen and (min-width: 900px) {
            font-size: 21px;
            display: flex;
            justify-content: space-around;
            align-content: center;
            .icons {
                margin: 45px 40px 35px 40px;
            }
        }
        img {
            width: 25px;
            opacity: 0.6;
            margin-left:10px;
        }
        img:hover {
            opacity: 0.9;
            cursor: pointer;
        }
    }
}
</style>