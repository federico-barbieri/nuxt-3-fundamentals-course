<template>
    <div>

        <main>

            <section class="hero">

                <Name class="name" />

                <ProjectSquare class="projectSquare" />

                <h2 class="about-title"> <nuxt-link to="/about">ABOUT</nuxt-link></h2>

                <Dog class="dog" />

                <p class="about-p">
                    I'm a Frontend Developer with a background in advertising. <br>
                    I'm in my last semester at Københavns Erhvervsakademi (KEA) <br>
                    and currently doing an internship @ Waitly.dk
                </p>

                <NiceBackground class="nice-background" />

                <p class="about-p">
                    I enjoy trying out new tools that spark my curiosity <br>
                    and enhance my ideas.
                </p>

                <Random class="random" />

                <IconGallery :images="stackArray" />

                <h2 class="projects-title"> <nuxt-link to="/projects">PROJECTS</nuxt-link></h2>

                <ProjectCard 
                        class="messiverse"  
                        name="Messiverse" 
                        description="Dive into this personal project where I explore <br>how different painters from history would have <br>recreated Argentina winning the World Cup" 
                        img="/projectImgs/messi.png"
                        :stack="['/icons/vuejs.png', '/icons/vitejs.png', '/icons/openai.png']"
                        border_bottom="1px solid white"
                        border_top="none"
                        margin="0 10rem 10rem 2rem"
                />

                <ProjectCard 
                        class="swampfest" 
                        name="SwampFest"  
                        description="The best festival in the world" 
                        img="/projectImgs/shrek.jpg"
                        :stack="['/icons/nextjs2.png', '/icons/git.png', '/icons/typescript.png']"
                        border_bottom="none"
                        border_top="1px solid white"
                        margin="10rem 10rem 2rem 2rem"
                />

                <ProjectCard 
                        class="hackers" 
                        name="Magic Hackers"  
                        description="A dashboard for Dumbledore" 
                        img="/projectImgs/hogwarts.png"
                        :stack="['/icons/ai.svg', '/icons/ps.svg', '/icons/js.svg']"
                        border_bottom="1px solid white"
                        border_top="none"
                        margin="0 10rem 10rem 2rem"
                />

                <ProjectCard 
                        class="edc" 
                        name="EDC"  
                        description="Find the house of your dreams" 
                        img="/projectImgs/ecd.jpg"
                        :stack="['/icons/xd.svg', '/icons/figma.svg', '/icons/reactjs.svg']"
                        border_bottom="none"
                        border_top="1px solid white"
                        margin="10rem 10rem 2rem 2rem"
                        
                />

                <h2 class="contact-title">CONTACT</h2>
                <p>Let's get in touch and start something memorable together.</p>

               
            </section>
            
               
        </main>

</div>
</template>

<script setup>

import Button from "../components/Button.vue";
import stack from "../assets/stack.json"
import Name from "../components/Name.vue";
import ProjectSquare from "../components/ProjectSquare.vue";
import Random from "../components/Random.vue";
import Dog from "../components/Dog.vue";
import NiceBackground from "../components/NiceBackground.vue";

let stackArray = stack.stack;



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
    height: 85vh;
    color: var(--near-white);
    display: flex;
    flex-direction: column;
    font-family: 'Raleway', sans-serif;
    background-color: rgb(17,17,17);
    white-space: nowrap; /* Prevent text from wrapping */
    overflow-x: auto; /* Enable horizontal scrolling when needed */
    overflow-y: hidden;
}

/* HERO */

.hero{
    display: flex;
    flex-direction: row;
    align-items: center;
    height: 85vh;
    width: 600vw;
    border: 1px solid white;
    margin: auto auto;
    border-radius: 30px;
    padding: 2rem;
    
}


h2{
    font-size: 5rem;
    opacity: 0.3;
    margin: 0 5vw;
}

/* ABOUT */
.about-title{
    writing-mode: vertical-rl; /* vertical writing mode, right-to-left */
    text-orientation: upright; /* characters are upright */
}

.about-p{
    font-size: 1rem;
    margin: 0rem 0 0 2rem;
    width: 40rem;
    height: 50%;
    line-height: 2;
    display: flex;
    align-items: center;
}


.projects-title{
    writing-mode: vertical-rl; /* vertical writing mode, right-to-left */
    text-orientation: upright; /* characters are upright */
    font-size: 3rem;
}

.p-and-ul{
    width: 70%;
    height: 100%;
    text-align: center;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: space-around;
}

.projects-p{
    font-size: 1.5rem;
}

/* list of projects */
.project-list{
    list-style-type: none;
    display: grid;
    grid-template-columns: 1fr 1fr;
    grid-template-rows: 1fr 1fr;
    height: 35%;
    width: 100%;
}

.project-img{
    max-width: 100%;
    height: auto;
    border-radius: 5px;
    filter: drop-shadow(5px 5px 5px black);
}

/* STACK */

.stack{
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: space-around;
    height: 250vh;
    width: 100%;
    padding: 1rem;
    margin: 1rem;
}

.stack-title{
    writing-mode: vertical-rl; /* vertical writing mode, right-to-left */
    text-orientation: upright; /* characters are upright */
    width: 30%;
}

.p-and-ul-stack{
    width: 70%;
    height: 100%;
    text-align: center;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
}

.stack-p{
    font-size: 1.5rem;
    max-width: 50%;
    margin: 0 0 10rem 0;
}

/* list of projects */
.stack-list{
    list-style-type: none;
    display: grid;
    grid-template-columns: 1fr 1fr 1fr;
    grid-template-rows: repeat(6, 1fr);
    height: 60%;
    width: 100%;
    gap: 1rem;
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