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
                <span> - </span>
                <span class='section' @click="scrollToWritings">WRITINGS</span>
                <span> - </span>
                <span class='section'>DRAWINGS</span>
                <span> - </span>
                <span class='section'>CONTACT</span>
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
        }
    }
}
</script>

<style lang="scss">
.about {
    height: 75vh;
    padding: 260px 10% 0 10%;
    .info {
        background-color: white;
        padding: 5% 12%;
        nav {
            padding-top: 20px;
            span {
                margin: 2%;
            }
            .section:hover {
                color: black;
            }
        }
    }
}
</style>