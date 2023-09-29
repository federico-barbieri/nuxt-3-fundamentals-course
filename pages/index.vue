<template>
    <div>

        <main>

            <section class="hero">

                <h1><span class="federico">FEDERICO</span> <span class="barbieri">BARBIERI</span></h1>

                <a :href="`#${scrollToElementId}`">
                 <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-arrow-right arrow-name" viewBox="0 0 16 16">
                    <path fill-rule="evenodd" d="M1 8a.5.5 0 0 1 .5-.5h11.793l-3.147-3.146a.5.5 0 0 1 .708-.708l4 4a.5.5 0 0 1 0 .708l-4 4a.5.5 0 0 1-.708-.708L13.293 8.5H1.5A.5.5 0 0 1 1 8z"/>
                </svg>
                </a>

                <div class="messi-container" :id="scrollToElementId">
        
                    <img class="messi-image" src="/projectImgs/messi.png" alt="Project image">
                    
                    <p class="about-p">
                    I'm a Frontend Developer with a background in advertising. <br>
                    I'm in my last semester at Københavns Erhvervsakademi (KEA) <br>
                    and currently doing an internship @ Waitly.dk
                    </p>

                </div>    

                

                <NiceBackground class="nice-background" />

                <p class="about-p">
                    I enjoy trying out new tools that spark my curiosity <br>
                    and enhance my ideas.
                </p>

                <Random class="random" />

                <IconGallery class="iconGallery" :images="stackArray" />

                <h2 class="projects-title">PROJECTS</h2>


                <ProjectCard 
                        class="swampfest" 
                        name="SwampFest"  
                        description="Experience the first Shrek-themed music festival in the world.<br> Get your tickets, add-ons and much more in this 7-day festival." 
                        :stack="['/icons/nextjs2.png', '/icons/git.png', '/icons/typescript.png']"
                        border_bottom="none"
                        border_top="1px solid white"
                        margin="10rem 10rem 2rem 2rem"
                        liveProject="/swampfest"
                />

                <ProjectCard 
                        class="messiverse"  
                        name="Messiverse" 
                        description="Dive into this personal project where I explore <br>how different painters from history would have <br>recreated Argentina winning the World Cup" 
                        :stack="['/icons/vuejs.png', '/icons/vitejs.png', '/icons/openai.png']"
                        border_bottom="1px solid white"
                        border_top="none"
                        margin="0 10rem 10rem 2rem"
                        liveProject="https://messiverse-omega.vercel.app/"
                />

                <ProjectCard 
                        class="edc" 
                        name="EDC"  
                        description="Find the house of your dreams, whether it's an urban villa or a cottage in the countryside. <br>Pick your favorites and we will take care of the rest." 
                        :stack="['/icons/xd.svg', '/icons/figma.svg', '/icons/reactjs.svg']"
                        border_bottom="none"
                        border_top="1px solid white"
                        margin="10rem 10rem 2rem 2rem"
                        liveProject="https://vercel.com/federico-barbieri/charlie-tango-case"
                        
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

let scrollToElementId = 'messi-container';





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
    width: 800vw;
    margin: auto 15rem auto 0;
    border-radius: 30px;
    padding: 2rem;
    
}

h1{
    font-size: 8rem;
    margin-bottom: 1rem;
}

.arrow-name{
    transform: scale(6);
    margin-left: 7rem;
}

.messi-container{
    width: 90vw;
    height: 80vh;
    background-color: transparent;
    border-bottom-left-radius: 30px;
    border-bottom-right-radius: 30px;
    font-family: 'Raleway', sans-serif;
    text-align: center;
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: center;
    margin: 1rem 0 0rem 10rem;
}

.messi-image{
    max-width: 30%;
    height: auto;
    border-bottom-left-radius: 30px;
    border-bottom-right-radius: 30px;
    transform: scale(0.8);
}


h2{
    font-size: 6rem;
    opacity: 0.3;
    margin: 0 5vw;
}

/* ABOUT */
.about-title{
    writing-mode: vertical-rl; /* vertical writing mode, right-to-left */
    text-orientation: upright; /* characters are upright */
}

.about-p{
    font-size: 1.5rem;
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
    font-size: 5rem;
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

.iconGallery{
    margin-right: 10rem;
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

.swampfest{
    transition: all 0.5s ease-in;
}

.swampfest:hover{
    background-image: url('/projectImgs/festival1.jpg');
    background-position: center;
    background-size: cover;
    background-repeat: no-repeat;
    backface-visibility: hidden;
    color: black;
    font-weight: 700;
}


.messiverse{
    transition: all 0.5s ease-in;
}

.messiverse:hover{
    background-image: url('/messi/xul1.png');
    background-position: center;
    background-size: cover;
    background-repeat: no-repeat;
    backface-visibility: hidden;
    color: black;
    font-weight: 700;
}

.sakurai{
    transition: all 0.5s ease-in;
}

.sakurai:hover{
    background-image: url('/projectImgs/moon.png');
    background-position: center;
    background-size: cover;
    background-repeat: no-repeat;
    backface-visibility: hidden;
    color: black;
    font-weight: 700;
}

.hogwarts{
    transition: all 0.5s ease-in;
}

.hogwarts:hover{
    background-image: url('/projectImgs/fire-hogwarts.png');
    background-position: center;
    background-size: cover;
    background-repeat: no-repeat;
    backface-visibility: hidden;
    color: black;
    font-weight: 700;
}

.edc{
    transition: all 0.5s ease-in;
}

.edc:hover{
    background-image: url('/projectImgs/ecd.jpg');
    background-position: center;
    background-size: cover;
    background-repeat: no-repeat;
    backface-visibility: hidden;
    color: black;
    font-weight: 700;
}

</style>