<template>
    <div class='about'>
        <div class='info'>
            <h2>Software Developer</h2>
            <p>
                Full stack developer, passionate creator, curious learner.
                I have a background in Multimedia, Design and Journalism.
                Experienced in Ruby on Rails, JavaScript, React, Node and Vue. 
                A contributing writer for The Startup.
            </p>
            <nav>
                <span class='section' @click="scrollToProjects">PROJECTS</span>
                <span class='dash'> - </span>
                <span class='section' @click="scrollToWritings">WRITINGS</span>
                <span class='dash'> - </span>
                <span class='section' @click="scrollToDrawings">DRAWINGS</span>
                <span class='dash'> - </span>
                <span class='section' @click="scrollToContact">CONTACT</span>
            </nav>
        </div>
    </div>
</template>

<script>
export default {
    methods: {
        scrollToProjects() {
            let projects = document.querySelector('.projects')
            let projectsOffset = 190
            let projectsPosition = projects.getBoundingClientRect().top
            let offsetPosition = projectsPosition - projectsOffset
            window.scrollTo({
                top: offsetPosition,
                behavior: 'smooth'
            })
        },
        scrollToWritings() {
            let writings = document.querySelector('.writings')
            let writingsOffset = 135
            let writingsPosition = writings.getBoundingClientRect().top
            let offsetPosition = writingsPosition - writingsOffset
            window.scrollTo({
                top: offsetPosition,
                behavior: 'smooth'
            })
        },
        scrollToDrawings() {
            let drawings = document.querySelector('.drawings')
            let drawingsOffset = 105
            let drawingsPosition = drawings.getBoundingClientRect().top
            let offsetPosition = drawingsPosition - drawingsOffset
            window.scrollTo({
                top: offsetPosition,
                behavior: 'smooth'
            })
        },
        scrollToContact() {
            let contact = document.querySelector('.contact')
            let contactOffset = 130
            let contactPosition = contact.getBoundingClientRect().top
            let offsetPosition = contactPosition - contactOffset
            window.scrollTo({
                top: offsetPosition,
                behavior: 'smooth'
            })
        }
    }
}
</script>

<style lang="scss">
.about {
    height: 70vh;
    @media screen and (min-width: 320px) {
        padding-top: 55%;
    }
    @media screen and (max-width: 570px) {
        padding-top: 65%;
    }
    @media screen and (min-width: 700px) {
        height: 75vh;
        padding: 260px 10% 0 10%;
    }
    @media screen and (max-height: 420px) {
        padding-top: 25%;
        padding-bottom: 20%;
    }
    @media screen and (max-height: 370px) {
        padding-top: 30%;
        padding-bottom: 20%;
    }
    .info {
        background-color: white;
        padding: 5% 12%;
        margin: auto;
        nav {
            padding-top: 20px;
            margin: auto;
            display: flex;
            flex-flow: row wrap;
            justify-content: space-evenly;
            span {
                margin: 2%;
                text-decoration: underline;
                @media screen and (min-width: 750px) {
                    text-decoration: none;
                }
            }
            .dash {
                display: none;
                @media screen and (min-width: 750px) {
                    display: inline-block;
                }
            }
            .section:hover {
                color: tan;
            }
        }
    }
}
</style>