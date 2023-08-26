<template>
    <div>

        <main>

            <section class="hero">

                <h1><span class="federico">FEDERICO</span> <span class="barbieri">BARBIERI</span></h1>
                <span class="frontend-developer">BETWEEN TWO HEMISPHERES</span>

            </section>

            <section class="about">

                <h2 class="about-title"> <nuxt-link to="/about">ABOUT</nuxt-link></h2>
                <p class="about-p">
                    I'm a Frontend Developer with a background in advertising.

                </p>

            </section>

            <section class="projects">
                
                <p>Check a selection of projects I've been working on over the past year</p>
                
                <ul class="project-list">
                    <ProjectCard name="Messiverse" description="a cool project" />
                    <ProjectCard name="Magic Hackers" description="a cool project" />
                    <ProjectCard name="Jimmy Sakurai" description="a cool project" />
                    <ProjectCard name="SwampFest" description="a cool project" />
                    
                </ul>
                <h2 class="projects-title"> <nuxt-link to="/projects">PROJECTS</nuxt-link></h2>
                
            </section>

            <section class="contact">
                <h2 class="contact-title">CONTACT</h2>
                <p>let's get in touch!</p>
            </section>

            


        </main>

</div>
</template>

<script setup>

import ProjectCard from "../components/ProjectCard.vue"

</script>

<style scoped>

a{
    color: inherit;
}

a:visited{
    color: inherit;
}

/* MAIN */

main{
    width: 100vw;
    height: auto;
    color: var(--near-white);
    display: flex;
    flex-direction: column;
    font-family: "Poppins", sans-serif;
    background-color: var(--neutral-gray);
    overflow: hidden;
}

/* HERO */

.hero{
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    height: 85vh;
    width: 100vw;
    border: 10px solid red;
}

h1{
    font-size: 5rem;
    text-align: center;
}

.federico{
    text-decoration: underline;
    display: inline-block;
    transform: translate(3rem, -5.39rem);
}

.barbieri{
    text-decoration: overline;
    display: inline-block;
    transform: translate(1.5rem, 0.61rem);
}

.frontend-developer{
    font-size: 1.5rem;
    display: block;
    margin: 3rem auto;
}

h2{
    font-size: 15rem;
    opacity: 0.3;
}

/* ABOUT */

.about{
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: space-around;
    height: auto;
    width: 100%;
    border: 10px solid green;

}

.about-title{
    writing-mode: vertical-rl; /* vertical writing mode, right-to-left */
    text-orientation: upright; /* characters are upright */
}

.about-p{
    font-size: 1.5rem;
    margin-left: 2rem;
}




/* PROJECTS */

.projects{
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: space-around;
    height: auto;
    width: 100%;
}

.projects-title{
    writing-mode: vertical-rl; /* vertical writing mode, right-to-left */
    text-orientation: upright; /* characters are upright */
}

/* list of projects */
.project-list{
    list-style-type: none;
}

/* CONTACT */

.contact{
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    height: 85vh;
    width: 100%;
}

.contact-title{
    
    text-decoration: overline;
}

</style>