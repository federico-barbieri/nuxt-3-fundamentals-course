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

                <div class="p-and-ul">

                    <p class="projects-p">Check a selection of projects I've been working on over the past year</p>
                
                    <ul class="project-list">
                    
                    <ProjectCard name="Messiverse" description="a cool project" img="/projectImgs/messi.png"  />
                    <ProjectCard name="Magic Hackers" description="A dashboard for Dumbledore" img="/projectImgs/fire-hogwarts.png" />
                    <ProjectCard name="Jimmy Sakurai" description="A tribute to a great guitar player" img="/projectImgs/moon.png" />
                    <ProjectCard name="SwampFest" description="The best festival in the world" img="/projectImgs/shrek.jpg" />

                    
                    </ul>



                </div>
                
               
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

}

.about-title{
    writing-mode: vertical-rl; /* vertical writing mode, right-to-left */
    text-orientation: upright; /* characters are upright */
}

.about-p{
    font-size: 1.5rem;
    margin: 10rem 0 0 2rem;
}




/* PROJECTS */

.projects{
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: space-around;
    height: 250vh;
    width: 100%;
    padding: 1rem;
    margin: 1rem;
}

.projects-title{
    writing-mode: vertical-rl; /* vertical writing mode, right-to-left */
    text-orientation: upright; /* characters are upright */
    width: 30%;
}

.p-and-ul{
    width: 70%;
    height: 100%;
    text-align: center;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: flex-end;
}

.projects-p{
    font-size: 1.5rem;
}

/* list of projects */
.project-list{
    list-style-type: none;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: space-around;
    height: 80%;
    width: 100%;
}

/* CONTACT */

.contact{
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    height: 100vh;
    width: 100%;
}

.contact-title{
    
    text-decoration: overline;
}

</style>