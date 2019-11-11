<template>
    <div >
        <div class='home'>
            <header>
                <h1 >CATHERINE O'HARA</h1>
                <div class='icons'>
                    <img src='../assets/icons/linkedinlogo.svg' @click='openLinkedIn' alt='LinkedIn'>
                    <img src='../assets/icons/githublogo.svg' @click='openGitHub' alt='GitHub'>
                    <img src='../assets/icons/mediumlogo.svg' @click='openMedium' alt='Medium'>
                    <img src='../assets/icons/twitterlogo.svg' @click='openTwitter' alt='Twitter'>
                    <img src='../assets/icons/resumelogo.svg' @click='openResume' alt='Resume'>
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
    },
    methods: {
        openLinkedIn() {
            window.open('https://www.linkedin.com/in/catherine-o/', '_blank')
        },
        openGitHub() {
            window.open('https://github.com/catherine-o', '_blank')
        },
        openMedium() {
            window.open('https://medium.com/@oharacatherine', '_blank')
        },
        openTwitter() {
            window.open('https://twitter.com/catherine__oh', '_blank')
        },
        openResume() {
            window.open('https://docs.google.com/presentation/d/13KNWovJC7EkSLTLU-HEQKly9R2E4Xvr9a0UGxvnCyC8/edit?usp=sharing', '_blank')
        }
    }
}
</script>

<style lang="scss">
.home {
      background-image: url('../assets/leaves.jpeg');
      background-position: center;
      background-attachment: fixed;
      background-repeat: no-repeat;
      width: 100%;
      height: 100vh;
      header {
          font-family: 'Montserrat', sans-serif;
          letter-spacing: 2px;
          background-color:rgb(231, 223, 216);
          position: fixed;
          padding: 14px;
          text-align: center;
          z-index: 3;
          font-size: 20px;
          @media screen and (min-width: 500px) {
            padding: 14px;
            width: 100vw;
          }
          @media screen and (min-width: 900px) {
            font-size: 21px;
            display: flex;
            justify-content: space-around;
            align-content: center;
            .icons {
                margin: 40px 10px;
            }
          }
            img {
                width: 25px;
                opacity: 60%;
                margin-left:10px;
            }
            img:hover {
                opacity: 90%;;
            }
      }
    //   .sections {
    //       background: none;
    //     //   padding: 260px 10%;
    // }
}
</style>