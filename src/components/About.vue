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
                <span class='section' @click='scrollToProjects'>PROJECTS</span>
                <span> - </span>
                <span class='section'>WRITINGS</span>
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
            
        }
    }
}
</script>

<style lang="scss">
.about {
    height: 80vh;
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