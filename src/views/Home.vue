<template>
    <div class='home'>
        <h1 id='name'>Catherine O'Hara</h1>
        <About />
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
      #name {
          background-color:white;
      }
}
</style>