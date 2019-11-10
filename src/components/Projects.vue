<template>
    <div class='projects'>
        <h2>PROJECTS</h2>
        <div class='project-grid'>
            <div class='project-profile'>
                <img id='app-img' src='../assets/greenhouse.png' alt='GreenHouse App'>
                <p> 
                    <b>GreenHouse</b> 
                    <br>
                    A plant service on request app inspired by <br>
                    business models of popular on-demand service apps
                    <br><br>
                    Built with: <br>
                    Vanilla JavaScript, Ruby on Rails <br>
                    SQLite and WeatherWidget.io
                </p>
                <img class='icons' src='../assets/icons/githublogo.svg' alt='GitHub'>
            </div>
            
            <div class='project-profile'>
                <img id='app-img' src='../assets/enroute.png' alt='En Route App'>
                <p> 
                    <b>En Route</b> 
                    <br>
                    A personal guide to the U.S. National Parks that <br>
                    tracks parks a user has or would like to visit
                    <br><br>
                    Built with: <br>
                    React.js, Ruby on Rails <br>
                    PostgreSQL and Google Maps API
                </p>
                <img class='icons' src='../assets/icons/githublogo.svg' alt='GitHub'>
            </div>

            <div class='project-profile'>
                <img id='app-img' src='../assets/sensi.png' alt='Sensi App'>
                <p> 
                    <b>Sensi</b> 
                    <br>
                    An interactive journal experience that <br>
                    provides insight to and engages human emotions
                    <br><br>
                    Built with: <br>
                    Vue.js, Node.js, Express.js <br>
                    PostgreSQL, Vuex
                </p>
                <img class='icons' src='../assets/icons/githublogo.svg' alt='GitHub'>
            </div>
            
            <div class='project-profile trivia-app'>
                <img id='trivia-img' src='../assets/trivia.png' alt='Trivia App'>
                <p> 
                    <b>Trivia Time!</b> 
                    <br>
                    A multiple-choice trivia game that keeps track <br>
                    of team scores on scoreboard. A collaboration project.
                    <br><br>
                    Built with: <br>
                    Ruby on Rails and SQLite <br>
                    <br>
                </p>
                <img class='icons' src='../assets/icons/githublogo.svg' alt='GitHub'>
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
.projects {
    height: 35vh;
    @media screen and (min-width: 1000px) {
        .project-grid {
            display: flex;
            flex-flow: row wrap;
            justify-content: space-evenly;
        }
    }
    .project-profile {
        margin: 35px auto;
    }
    #app-img {
        width: 500px;
    }
    #trivia-img {
        width: 500px;
        height: 312px;
    }
    .icons {
        width: 25px;
        opacity: 60%;
        margin-left:10px;
    }
    .icons:hover {
        opacity: 90%;;
    }
    .arrows {
        width: 25px;
        opacity: 60%;
        position: relative;
        top: 70%;
        left: 50%;
    }
    .arrows:hover {
        opacity: 90%;;
    }
}
</style>