<template>
    <div >
        <div class='home'>
            <header>
                <h1 >CATHERINE O'HARA</h1>
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
          font-family: 'Montserrat', sans-serif;
          letter-spacing: 2px;
          background-color:rgb(231, 223, 216);
          position: fixed;
          width: 100%;
          margin-top: 0;
          padding: 14px;
          font-size: 21px;
          text-align: center;
          @media screen and (min-width: 900px) {
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
      .element {
          background: none;
          padding: 230px 10%;
    }
}
</style>