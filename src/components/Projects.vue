<template>
    <div class='projects'>
        <h2>PROJECTS</h2>
        <div class='project-grid'>
            <div class='project-profile'>
                <a href='https://github.com/catherine-o/GreenHouse' target='_blank'>
                    <img id='app-img' src='../assets/projects/greenhouse.png' alt='GreenHouse App'>
                </a>
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
                <img class='icons' @click='openGreenHouseGitHub' src='../assets/icons/githublogo.png' alt='GitHub'>
                <img class='icons' @click='openGreenHouseVideo' src='../assets/icons/youtubelogo.svg' alt='GreenHouse on YouTube'>
            </div>
            
            <div class='project-profile'>
                <a href='https://github.com/catherine-o/national-parks-frontend' target='_blank'>
                    <img id='app-img' src='../assets/projects/enroute.png' alt='En Route App'>
                </a>
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
                <img class='icons' @click='openEnRouteGitHub' src='../assets/icons/githublogo.png' alt='GitHub'>
                <img class='globe-icon' @click='openEnRouteWebpage' src='../assets/icons/globeicon.png' alt='Demo'>
                <img class='icons' @click='openEnRouteVideo' src='../assets/icons/youtubelogo.svg' alt='En Route on YouTube'>
            </div>

            <div class='project-profile'>
                <a href='https://github.com/catherine-o/sensi-frontend' target='_blank'>
                    <img id='app-img' src='../assets/projects/sensi.png' alt='Sensi App'>
                </a>
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
                <img class='icons' @click='openSensiGitHub' src='../assets/icons/githublogo.png' alt='GitHub'>
                <img class='icons' @click='openSensiVideo' src='../assets/icons/youtubelogo.svg' alt='En Route on YouTube'>
            </div>
            
            <div class='project-profile trivia-app'>
                <a href='https://github.com/catherine-o/TriviaTime' target='_blank'>
                    <img id='trivia-img' src='../assets/projects/trivia.png' alt='Trivia App'>
                </a>
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
                <img class='icons' @click='openTriviaGitHub' src='../assets/icons/githublogo.png' alt='GitHub'>
                <img class='icons' @click='openTriviaVideo' src='../assets/icons/youtubelogo.svg' alt='En Route on YouTube'>
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
        },
        openGreenHouseGitHub() {
            window.open('https://github.com/catherine-o/GreenHouse', '_blank')
        },
        openGreenHouseVideo() {
            window.open('https://www.youtube.com/watch?v=-JK8fxub4ek&feature=youtu.be', '_blank')
        },
        openEnRouteGitHub() {
            window.open('https://github.com/catherine-o/national-parks-frontend', '_blank')
        },
        openEnRouteWebpage() {
            window.open('https://national-parks-app.web.app/login', '_blank')
        },
        openEnRouteVideo() {
            window.open('https://www.youtube.com/watch?v=WzjgFscnQqE', '_blank')
        },
        openSensiGitHub() {
            window.open('https://github.com/catherine-o/sensi-frontend', '_blank')
        },
        openSensiVideo() {
            window.open('https://www.youtube.com/watch?v=V5oDAX56trY', '_blank')
        },
        openTriviaGitHub() {
            window.open('https://github.com/catherine-o/TriviaTime', '_blank')
        },
        openTriviaVideo() {
            window.open('https://www.youtube.com/watch?v=Gq7AQbAOsg8', '_blank')
        }
    }
}
</script>

<style lang="scss">
.projects {
    padding: 0 30px 30px 30px;
    @media screen and (min-height: 1000px) {
        margin-top: 120px;
    }
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
        width: 95%;
        @media screen and (min-width: 1000px) {
            width: 500px;
        }
    }
    #app-img:hover {
        cursor: pointer;
    }
    #trivia-img {
        width: 95%;
        @media screen and (min-width: 1000px) {
            height: 312px;
            width: 500px;
        }
    }
    .icons {
        width: 25px;
        opacity: 0.6;
        margin-left:10px;
    }
    .icons:hover {
        opacity: 0.9;
        cursor: pointer;
    }
    .globe-icon {
        width: 25px;
        opacity: 0.8;
        margin-left:10px;
    }
    .globe-icon:hover {
        opacity: 1;
        cursor: pointer;
    }
    .arrows {
        width: 25px;
        opacity: 0.6;
        position: relative;
        top: 60%;
        left: 45%;
        @media screen and (min-height: 1000px) {
            left: 43%;
        }
    }
    .arrows:hover {
        opacity: 0.9;
        cursor: pointer;
    }
}
</style>