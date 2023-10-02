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
                    I'm a multimedia design student at KEA <br>with a focus in frontend design and a background in advertising. 
                    </p>

                </div>    

                <div class="medieval-container">
        
                        <img class="medieval-background" src="/random/nice-background.webp" alt="Project image">
                        
                        <p class="medieval-p">
                        I enjoy trying out new tools that spark my curiosity <br>
                        and enhance my ideas.
                        </p>

                </div>  

                <div class="mondrian-container">
        
                    <video
                        class="mondrian"
                        ref="loopingVideo"
                        autoplay
                        muted
                        loop
                    >
                         <source src="/random/mondrian-2.webm" type="video/webm">
                    </video>
                    

                </div> 

                <IconGallery class="iconGallery" :images="stackArray" />

                <h2 class="projects-title" id="projects">PROJECTS</h2>

                <ProjectCard 
                        class="messiverse"  
                        name="Advertising" 
                        description="Over the years, I have worked with<br>many different brands in international multimedia campaigns.<br>Take a look at some of my work." 
                        :stack="['/icons/ai.svg', '/icons/ps.svg', '/icons/ae.png']"
                        border_bottom="1px solid white"
                        border_top="none"
                        margin="0 10rem 10rem 2rem"
                        liveProject="/advertising"
                />


                <ProjectCard 
                        id="swampfest-project"
                        class="swampfest" 
                        name="SwampFest"  
                        description="Experience the first Shrek-themed music festival in the world.<br> Get your tickets, add-ons and much more in this 7-day festival." 
                        :stack="['/icons/nextjs2.png', '/icons/git.png', '/icons/typescript.png']"
                        border_bottom="none"
                        border_top="1px solid white"
                        margin="10rem 10rem 2rem 2rem"
                        liveProject="/swampfest"
                />


            <!--    <ProjectCard 
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
                        
                /> -->

                <h2 class="contact-title">CONTACT</h2>
                <p>Let's get in touch and start something memorable together.</p>

               
            </section>
            
               
        </main>

</div>
</template>

<script setup>

import stack from "../assets/stack.json"
import Random from "../components/Random.vue";

import { ref, onMounted } from 'vue';

// mondrian

const loopingVideo = ref(null);

onMounted(() => {
      // Access the video element and play it
      loopingVideo.value.play();
    });


// icon gallery

let stackArray = stack.stack;


// messi container

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
    width: 550vw;
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

/* messi container */

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

.about-p{
    font-size: 1.5rem;
    margin: 0rem 0 0 2rem;
    width: 40rem;
    height: 50%;
    line-height: 2;
    display: flex;
    text-align: left;
}

/* medieval container */

.medieval-container{
    width: 90vw;
    height: 80vh;
    background-color: transparent;
    border-bottom-left-radius: 30px;
    border-bottom-right-radius: 30px;
    font-family: 'Raleway', sans-serif;
    text-align: center;
    display: flex;
    flex-direction: row;
    align-items: flex-end;
    justify-content: center;
    margin: 1rem 0 0rem 10rem;
}

.medieval-background{
    max-width: 80%;
    height: auto;
    border-bottom-left-radius: 30px;
    border-bottom-right-radius: 30px;
    transform: scale(0.8);
}

.medieval-p{
    font-size: 1.5rem;
    margin: 0rem 0 0 2rem;
    width: 40rem;
    height: 50%;
    line-height: 2;
    display: flex;
    text-align: left;
}

/* mondrian container */
.mondrian-container{
    width: 60vw;
    height: 70vh;
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

.mondrian{
    max-width:60%;
    height: auto;
    border-bottom-left-radius: 30px;
    border-bottom-right-radius: 30px;
}




.projects-title{
    writing-mode: vertical-rl; /* vertical writing mode, right-to-left */
    text-orientation: upright; /* characters are upright */
    font-size: 5rem;
}

.iconGallery{
    margin-right: 10rem;
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


</style>