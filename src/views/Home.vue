<template>
    <div >
        <div class='home'>
            <header>
                <h1 >Catherine O'Hara</h1>
                <div class='icons'>
                    <img src='../assets/icons/linkedinlogo.svg' alt='LinkedIn'>
                    <img src='../assets/icons/githublogo.svg' alt='GitHub'>
                    <img src='../assets/icons/mediumlogo.svg' alt='Medium'>
                    <img src='../assets/icons/twitterlogo.svg' alt='Twitter'>
                    <img src='../assets/icons/resumelogo.svg' alt='Resume'>
                </div>
            </header>
            <div class='element'>
                <About />
            </div>
        </div>
    </div>
</template>

<script>
import About from '@/components/About'
export default {
    components: {
        About
    }
}
</script>

<style lang="scss">
.home {
      background-image: url('../assets/leaves.jpeg');
      background-position: center;
      background-attachment: fixed;
      background-repeat: no-repeat;
      width: 100vw;
      height: 100vh;
      header {
          background-color:rgb(231, 223, 216);
          position: fixed;
          width: 100%;
          margin-top: 0;
          padding: 15px;
          font-size: 17px;
          text-align: center;
          @media screen and (min-width: 800px) {
            display: flex;
            justify-content: center;
            padding-left: 24.5%;
            .icons {
                margin: 40px 18% 1% 18%;
            }
          }
            img {
                width: 25px;
                opacity: 60%;
                margin-left:10px;
            }
      }
      .element {
          background: none;
          padding: 55% 10%;
          @media screen and (min-width: 500px) {
          padding: 25% 15%;
          }
          @media screen and (min-width: 800px) {
            padding: 15% 10%;
        }
    }
}
</style>