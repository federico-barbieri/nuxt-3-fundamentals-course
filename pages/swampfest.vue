<template>
    <div>

        <main>

            <section class="hero">

                <div class="title-container">

                    <h1><span class="federico">SWAMPFEST</span></h1>

                    <a :href="`#${scrollToElementId}`">
                        <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-arrow-right arrow-name" viewBox="0 0 16 16">
                            <path fill-rule="evenodd" d="M1 8a.5.5 0 0 1 .5-.5h11.793l-3.147-3.146a.5.5 0 0 1 .708-.708l4 4a.5.5 0 0 1 0 .708l-4 4a.5.5 0 0 1-.708-.708L13.293 8.5H1.5A.5.5 0 0 1 1 8z"/>
                        </svg>
                    </a>


                </div>


                <div class="burger-container" :id="scrollToElementId">
        
                    <img class="burger-image" src="/swampfest-gifs/burger.gif" alt="Gif of burger menu display">
                    
                    <p class="about-p">
                    This Shrek-inspired music festival<br>
                    is the final project of my 3rd semester at KEA.<br>
                    </p>

                </div>    

                <div class="schedule-container">

                    <img class="schedule-image" src="/swampfest-gifs/schedule.gif" alt="Gif of schedule page">

                    <p class="about-p">
                    The platform fetches information from an api<br>
                    and updates the schedule for three different stages<br>
                    in real-time.
                    </p>


                </div>

                <div class="bands-container">

                    <img class="bands-image" src="/swampfest-gifs/bands.gif" alt="Gif of bands page">

                    <p class="about-p">
                    You can also find a list of the bands<br>
                    that will be playing, their image, description<br>
                    and band members.
                    </p>


                </div>

                <div class="tickets-container">

                    <img class="tickets-image" src="/swampfest-gifs/ticket1.gif" alt="Gif of ticket step">

                    <p class="about-p">
                    The buying flow for tickets consists of 5 steps:<br>
                    tickets, camping add-ons, ticket-holder-information<br>
                    delivery and order review.
                    </p>


                </div>

                <div class="supabase-container">

                    <img class="supabase-image" src="/swampfest-gifs/supabase.png" alt="Supabase image">

                    <p class="about-p">
                    The project is connected to Supabase,<br>
                    so all the information is received<br>
                    in the correct format.
                    </p>


                </div>


                <h2 class="projects-title">PROCESS</h2>

                <div class="process-container">

                    <p class="about-p">
                        After doing research on current trends<br>
                        and famous music festivals,<br>
                        we agreed on the different sections of the website. 
                    </p>

                    <img class="process-one-image" src="/swampfest-gifs/user-flow-diagram.png" alt="User flow diagram">

                    <img class="process-two-image" src="/swampfest-gifs/bands-proto.png" alt="Band page early design">

                    <img class="process-three-image" src="/swampfest-gifs/timeline.png" alt="Schedule page early design">

                        


                </div>


                <h3 class="contact-title">GO TO LIVE WEBSITE</h3>
               <nuxt-link to="https://swampfest.vercel.app/" target="_blank">  <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-box-arrow-in-up-right" viewBox="0 0 16 16">
                                <path fill-rule="evenodd" d="M6.364 13.5a.5.5 0 0 0 .5.5H13.5a1.5 1.5 0 0 0 1.5-1.5v-10A1.5 1.5 0 0 0 13.5 1h-10A1.5 1.5 0 0 0 2 2.5v6.636a.5.5 0 1 0 1 0V2.5a.5.5 0 0 1 .5-.5h10a.5.5 0 0 1 .5.5v10a.5.5 0 0 1-.5.5H6.864a.5.5 0 0 0-.5.5z"/>
                                <path fill-rule="evenodd" d="M11 5.5a.5.5 0 0 0-.5-.5h-5a.5.5 0 0 0 0 1h3.793l-8.147 8.146a.5.5 0 0 0 .708.708L10 6.707V10.5a.5.5 0 0 0 1 0v-5z"/>
                            </svg>
                </nuxt-link>

               
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

let scrollToElementId = 'burger-container';





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
    width: 900vw;
    margin: auto 15rem auto 0;
    border-radius: 30px;
    padding: 2rem;
    
}

.title-container{
    width: 80vw;
    display: flex;
    flex-direction: row;
    align-items: center;
}

h1{
    font-size: 8rem;
    margin: 0 3rem 0 8rem;
}

.arrow-name{
    transform: scale(6);
    margin-left: 7rem;
}

.burger-container{
    width: 90vw;
    height: 80vh;
    background-color: transparent;
    border-bottom-left-radius: 30px;
    border-bottom-right-radius: 30px;
    font-family: 'Raleway', sans-serif;
    text-align: center;
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    justify-content: center;
    margin: 1rem 0 0rem 10rem;
}

.burger-image{
    max-width: 50%;
    height: auto;
    border-bottom-left-radius: 30px;
    border-bottom-right-radius: 30px;
    transform: scale(0.8);
}

.schedule-container{
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

.schedule-image{
    max-width: 50%;
    height: auto;
    border-bottom-left-radius: 30px;
    border-bottom-right-radius: 30px;
    transform: scale(0.8);
}

.bands-container{
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

.bands-image{
    max-width: 50%;
    height: auto;
    border-bottom-left-radius: 30px;
    border-bottom-right-radius: 30px;
    transform: scale(0.8);
}

.tickets-container{
    width: 90vw;
    height: 80vh;
    background-color: transparent;
    border-bottom-left-radius: 30px;
    border-bottom-right-radius: 30px;
    font-family: 'Raleway', sans-serif;
    text-align: center;
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    justify-content: center;
    margin: 1rem 0 0rem 10rem;
}

.tickets-image{
    max-width: 50%;
    height: auto;
    border-bottom-left-radius: 30px;
    border-bottom-right-radius: 30px;
    transform: scale(0.8);
}

.supabase-container{
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

.supabase-image{
    max-width: 60%;
    height: auto;
    border-bottom-left-radius: 30px;
    border-bottom-right-radius: 30px;
    transform: scale(0.8);
}

.process-container{
    width: 300vw;
    height: 80vh;
    background-color: transparent;
    border-bottom-left-radius: 30px;
    border-bottom-right-radius: 30px;
    font-family: 'Raleway', sans-serif;
    text-align: center;
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: space-around;
    margin: 1rem 0 0rem 0rem;
}

.process-one-image{
    max-width: 20%;
    height: auto;
    border-bottom-left-radius: 30px;
    border-bottom-right-radius: 30px;
    margin-bottom: 15rem;
}

.process-two-image{
    max-width: 15%;
    height: auto;
    border-bottom-left-radius: 30px;
    border-bottom-right-radius: 30px;
    margin-top: 15rem;
}

.process-three-image{
    max-width: 30%;
    height: auto;
    border-bottom-left-radius: 30px;
    border-bottom-right-radius: 30px;
    margin-bottom: 15rem;
}

h2{
    font-size: 6rem;
    opacity: 0.3;
    margin: 0 5vw;
}

h3{
    font-size: 3rem;
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