<template>
    <div>

        <main>

            <!-- HERO SECTION -->

            <section class="hero">

                <!-- TITLE CONTAINER -->

                <div class="title-container">

                    <div class="title-inner-div">
                        <h1><span class="federico">SWAMPFEST</span></h1>
                        <span>Made in collaboration with Sabrina Sørensen</span>

                    </div>

                    <a :href="`#${scrollToElementId}`">
                        <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-arrow-right arrow-name" viewBox="0 0 16 16">
                            <path fill-rule="evenodd" d="M1 8a.5.5 0 0 1 .5-.5h11.793l-3.147-3.146a.5.5 0 0 1 .708-.708l4 4a.5.5 0 0 1 0 .708l-4 4a.5.5 0 0 1-.708-.708L13.293 8.5H1.5A.5.5 0 0 1 1 8z"/>
                        </svg>

                        <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-arrow-down arrow-name-down" viewBox="0 0 16 16">
                            <path fill-rule="evenodd" d="M8 1a.5.5 0 0 1 .5.5v11.793l3.146-3.147a.5.5 0 0 1 .708.708l-4 4a.5.5 0 0 1-.708 0l-4-4a.5.5 0 0 1 .708-.708L7.5 13.293V1.5A.5.5 0 0 1 8 1z"/>
                        </svg>
                    </a>


                </div>

                <!-- BURGER MENU CONTAINER -->


                <div class="burger-container" :id="scrollToElementId">
        
                    <img class="burger-image" src="/swampfest-gifs/burger.gif" alt="Gif of burger menu display">
                    
                    <p class="burger-p">
                    This Shrek-inspired music festival
                    is the final project of my 3rd semester at KEA.
                    </p>

                </div>
                
                <!-- SCHEDULE CONTAINER -->

                <div class="schedule-container">

                    <img class="schedule-image" src="/swampfest-gifs/schedule.gif" alt="Gif of schedule page">

                    <p class="schedule-p">
                    The platform fetches information from an api
                    and updates the schedule for three different stages
                    in real-time.
                    </p>


                </div>

                <!-- BANDS CONTAINER -->

                <div class="bands-container">

                    <img class="bands-image" src="/swampfest-gifs/bands.gif" alt="Gif of bands page">

                    <p class="bands-p">
                    You can also find a list of the bands
                    that will be playing, their image, description
                    and band members.
                    </p>


                </div>

                <!-- TICKETS CONTAINER -->

                <div class="tickets-container">

                    <img class="tickets-image" src="/swampfest-gifs/ticket1.gif" alt="Gif of ticket step">

                    <p class="tickets-p">
                    The buying flow for tickets consists of 5 steps:
                    tickets, camping add-ons, ticket-holder-information
                    delivery and order review.
                    </p>


                </div>

                <!-- SUPABASE CONTAINER -->

                <div class="supabase-container">

                    <img class="supabase-image" src="/swampfest-gifs/supabase.png" alt="Supabase image">

                    <p class="supabase-p">
                    The project is connected to Supabase,
                    so all the information is received
                    in the correct format.
                    </p>


                </div>

                <!-- PROCESS TITLE -->


                <h2 class="process-title">WIREFRAMES</h2>

                <!-- PROCESS CONTAINER -->

                <div class="process-container">

                    <p class="process-p">
                        After doing research on current trends
                        and famous music festivals,
                        we agreed on the different sections of the website. 
                    </p>

                    <img class="process-one-image" src="/swampfest-gifs/user-flow-diagram.png" alt="User flow diagram">

                    <img class="process-two-image" src="/swampfest-gifs/bands-proto.png" alt="Band page early design">

                    <img class="process-three-image" src="/swampfest-gifs/timeline.png" alt="Schedule page early design">

                        


                </div>

                <div class="last-section">
                        
                        <nuxt-link to="https://swampfest.vercel.app/" target="_blank">  
                            <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-box-arrow-in-up-right see-website" viewBox="0 0 16 16">
                                <path fill-rule="evenodd" d="M6.364 13.5a.5.5 0 0 0 .5.5H13.5a1.5 1.5 0 0 0 1.5-1.5v-10A1.5 1.5 0 0 0 13.5 1h-10A1.5 1.5 0 0 0 2 2.5v6.636a.5.5 0 1 0 1 0V2.5a.5.5 0 0 1 .5-.5h10a.5.5 0 0 1 .5.5v10a.5.5 0 0 1-.5.5H6.864a.5.5 0 0 0-.5.5z"/>
                                <path fill-rule="evenodd" d="M11 5.5a.5.5 0 0 0-.5-.5h-5a.5.5 0 0 0 0 1h3.793l-8.147 8.146a.5.5 0 0 0 .708.708L10 6.707V10.5a.5.5 0 0 0 1 0v-5z"/>
                            </svg>
                        </nuxt-link>

                        <nuxt-link to="https://github.com/raptorp/foofest" target="_blank">
                            <img class="github-link" src="/icons/github.png" alt="Github logo">
                        </nuxt-link>

                        <a :href="`/#${backToProjects}`">
                            <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-arrow-return-left back-to-projects" viewBox="0 0 16 16">
                                <path fill-rule="evenodd" d="M14.5 1.5a.5.5 0 0 1 .5.5v4.8a2.5 2.5 0 0 1-2.5 2.5H2.707l3.347 3.346a.5.5 0 0 1-.708.708l-4.2-4.2a.5.5 0 0 1 0-.708l4-4a.5.5 0 1 1 .708.708L2.707 8.3H12.5A1.5 1.5 0 0 0 14 6.8V2a.5.5 0 0 1 .5-.5z"/>
                            </svg>
                        </a>



                </div>


               

               
            </section>
            
               
        </main>

</div>
</template>

<script setup>

let scrollToElementId = 'burger-container';

let backToProjects = 'swampfest-project';






</script>

<style scoped>

/* LINKS */

a{
    color: inherit;
}

a:visited{
    color: inherit;
}

/* TEXT */


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

/* HERO SECTION */

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

/* TITLE CONTAINER */

.title-container{
    width: 80vw;
    display: flex;
    flex-direction: row;
    align-items: center;
}

.title-inner-div{
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
}

h1{
    font-size: 8rem;
    margin: 0 3rem 0 8rem;
}

.arrow-name{
    transform: scale(6);
    margin-left: 7rem;
}


/* BURGER CONTAINER */

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

.burger-p{
    font-size: 1.5rem;
    margin: 0 auto;
    max-width: 50%;
    white-space: normal;
    height: auto;
    line-height: 2;
    text-align: left;
}

/* SCHEDULE CONTAINER */

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

.schedule-p{
    font-size: 1.5rem;
    margin: 0 auto;
    max-width: 50%;
    white-space: normal;
    height: auto;
    line-height: 2;
    text-align: left;
}


/* BANDS CONTAINER */

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

.bands-p{
    font-size: 1.5rem;
    margin: 0 auto;
    max-width: 50%;
    white-space: normal;
    height: auto;
    line-height: 2;
    text-align: left;
}


/* TICKETS CONTAINER */

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

.tickets-p{
    font-size: 1.5rem;
    margin: 0 auto;
    max-width: 50%;
    white-space: normal;
    height: auto;
    line-height: 2;
    text-align: left;
}


/* SUPABASE CONTAINER */

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

.supabase-p{
    font-size: 1.5rem;
    margin: 0 auto;
    max-width: 50%;
    white-space: normal;
    height: auto;
    line-height: 2;
    text-align: left;
}

/* PROCESS TITLE */

.process-title{
    writing-mode: vertical-rl; /* vertical writing mode, right-to-left */
    text-orientation: upright; /* characters are upright */
    font-size: 3rem;
    opacity: 0.3;
    margin: 0 5vw;
    color: white;
}


/* PROCESS CONTAINER */

.process-container{
    width: 180vw;
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

.process-p{
    font-size: 1.5rem;
    margin: 0 auto;
    max-width: 45ch;
    white-space: normal;
    height: auto;
    line-height: 2;
    text-align: left;
}

.process-one-image{
    max-width: 20%;
    height: auto;
    border-bottom-left-radius: 30px;
    border-bottom-right-radius: 30px;
    margin: 0 5rem 10rem 0;
}

.process-two-image{
    max-width: 15%;
    height: auto;
    border-bottom-left-radius: 30px;
    border-bottom-right-radius: 30px;
    margin: 10rem 5rem 0rem 0;

}

.process-three-image{
    max-width: 30%;
    height: auto;
    border-bottom-left-radius: 30px;
    border-bottom-right-radius: 30px;
    margin-bottom: 15rem;
    margin: 0rem 5rem 10rem 0;

}

/* LAST SECTION */

.last-section{
    width: 50vw;
    height: 80%;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: space-around;
    margin: 0 0 0 5rem;
}

.see-website{
    transform: scale(2);
}

.github-link{
    transform: scale(0.3);
}

.back-to-projects{
    transform: scale(2);
}


/* Tablet Styles */
@media screen and (min-width: 768px) and (max-width: 1300px) {
    main{
    width: 100vw;
    height: auto;
    color: var(--near-white);
    display: flex;
    flex-direction: column;
    font-family: 'Raleway', sans-serif;
    background-color: rgb(17,17,17);
    white-space:initial; /* Prevent text from wrapping */
    overflow-x: hidden; /* Enable horizontal scrolling when needed */
    overflow-y: auto;
}

/* HERO */

.hero{
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: space-around;
    height: auto;
    width: 100%;
    margin: auto;
    border-radius: 0;
    padding: 1rem;
}

.title-container{
    width: 90%;
    height: 80vh;
    background-color: transparent;
    border-bottom-left-radius: 0;
    border-bottom-right-radius: 0;
    font-family: 'Raleway', sans-serif;
    text-align: center;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    margin: 1rem 0 0rem 0rem;
}
h1{
    font-size: 5rem;
    margin: 0 0 2rem 0;
}
  .arrow-name{
    transform: scale(3);
    margin-left: 0rem;
    display: none;
}

.arrow-name-down{
    transform: scale(3);
    margin: 3rem 0 0 0;
    display: inline;
}

.burger-container{
    border: 1px solid white;
    width: 70%;
    height: auto;
    background-color: transparent;
    border-bottom-left-radius: 30px;
    border-bottom-right-radius: 30px;
    font-family: 'Raleway', sans-serif;
    text-align: center;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    margin: 0rem auto;
}

.burger-image{
    max-width: 100%;
}


.burger-p{
    font-size: 1rem;
    max-width: 70%;
    height: auto;
    line-height: 2;
    display: block;
    text-align: left;
    padding: 0 0 2rem 1rem;
}


/* medieval container */

.schedule-container{
    width: 70%;
    height: auto;
    background-color: transparent;
    border-bottom-left-radius: 30px;
    border-bottom-right-radius: 30px;
    font-family: 'Raleway', sans-serif;
    text-align: center;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    margin: 5rem 0 5rem 0rem;
}

.schedule-image{
    max-width: 100%;
    height: auto;
    border-top-left-radius: 30px;
    border-top-right-radius: 30px;
    border-bottom-left-radius: 0px;
    border-bottom-right-radius: 0px;
    transform: scale(1);
}

.schedule-p{
    font-size: 1rem;
    max-width: 100%;
    height: auto;
    line-height: 2;
    display: block;
    text-align: left;
    padding: 0 0 2rem 1rem;
    margin: 3rem auto;
}

.bands-container{
    border: 1px solid white;
    width: 70%;
    height: auto;
    background-color: transparent;
    border-bottom-left-radius: 30px;
    border-bottom-right-radius: 30px;
    font-family: 'Raleway', sans-serif;
    text-align: center;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    margin: 0rem auto;
}

.bands-image{
    max-width: 100%;
}


.bands-p{
    font-size: 1rem;
    max-width: 100%;
    height: auto;
    line-height: 2;
    display: block;
    text-align: center;
    padding: 0 0 2rem 1rem;
    margin: 0 auto;
}


.tickets-container{
    width: 90%;
    height: auto;
    background-color: transparent;
    border-bottom-left-radius: 30px;
    border-bottom-right-radius: 30px;
    font-family: 'Raleway', sans-serif;
    text-align: center;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    margin: 5rem auto;
}

.tickets-image{
    max-width: 100%;
}


.tickets-p{
    font-size: 1rem;
    max-width: 100%;
    height: auto;
    line-height: 2;
    display: block;
    text-align: center;
    padding: 0 0 2rem 1rem;
    margin: 0 auto;
}

.supabase-container{
    width: 70%;
    height: auto;
    background-color: transparent;
    border-bottom-left-radius: 30px;
    border-bottom-right-radius: 30px;
    font-family: 'Raleway', sans-serif;
    text-align: center;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    margin: 5rem 0 5rem 0rem;
}

.supabase-image{
    max-width: 100%;
    height: auto;
    border-top-left-radius: 30px;
    border-top-right-radius: 30px;
    border-bottom-left-radius: 0px;
    border-bottom-right-radius: 0px;
    transform: scale(1);
}

.supabase-p{
    font-size: 1rem;
    max-width: 100%;
    height: auto;
    line-height: 2;
    display: block;
    text-align: left;
    padding: 0 0 2rem 1rem;
    margin: 3rem auto;
}

.process-title{
    writing-mode: horizontal-tb; /* vertical writing mode, right-to-left */
    text-orientation: sideways-right; /* characters are upright */
    font-size: 3rem;
    opacity: 0.3;
    margin: 0 5vw;
    color: white;
}

.process-container{
    width: 90%;
    height: auto;
    background-color: transparent;
    border-bottom-left-radius: 30px;
    border-bottom-right-radius: 30px;
    font-family: 'Raleway', sans-serif;
    text-align: center;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: space-around;
    margin: 5rem auto;
}

.process-p{
    font-size: 1rem;
    margin: 2rem auto;
    max-width: 70%;
    white-space: normal;
    height: auto;
    line-height: 2;
    text-align: left;
}

.process-one-image{
    max-width: 70%;
    height: auto;
    border-bottom-left-radius: 30px;
    border-bottom-right-radius: 30px;
    margin: 2rem 13rem 0 0;
}

.process-two-image{
    max-width: 70%;
    height: auto;
    border-bottom-left-radius: 30px;
    border-bottom-right-radius: 30px;
    margin: 2rem 0 0 15rem;

}

.process-three-image{
    max-width: 90%;
    height: auto;
    border-bottom-left-radius: 30px;
    border-bottom-right-radius: 30px;
    margin: 2rem 0rem 0rem 0;
}


/* LAST SECTION */

.last-section{
    height: auto;
    width: 100%;
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: space-around;
}

.see-website{
    transform: scale(2);
}

.github-link{
    transform: scale(0.3);
}

.back-to-projects{
    transform: scale(2);
}
}




/* Mobile Styles */
@media screen and (max-width: 767px) {
    main{
    width: 100vw;
    height: auto;
    color: var(--near-white);
    display: flex;
    flex-direction: column;
    font-family: 'Raleway', sans-serif;
    background-color: rgb(17,17,17);
    white-space:initial; /* Prevent text from wrapping */
    overflow-x: hidden; /* Enable horizontal scrolling when needed */
    overflow-y: auto;
}

/* HERO */

.hero{
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: space-around;
    height: auto;
    width: 100%;
    margin: auto;
    border-radius: 0;
    padding: 1rem;
}

.title-container{
    width: 90%;
    height: 80vh;
    background-color: transparent;
    border-bottom-left-radius: 0;
    border-bottom-right-radius: 0;
    font-family: 'Raleway', sans-serif;
    text-align: center;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    margin: 1rem 0 0rem 0rem;
}
h1{
    font-size: 4rem;
    margin: 0 0 2rem 0;
}
  .arrow-name{
    transform: scale(3);
    margin-left: 0rem;
    display: none;
}

.arrow-name-down{
    transform: scale(3);
    margin: 3rem 0 0 0;
    display: inline;
}

.burger-container{
    border: 1px solid white;
    width: 100%;
    height: auto;
    background-color: transparent;
    border-bottom-left-radius: 30px;
    border-bottom-right-radius: 30px;
    font-family: 'Raleway', sans-serif;
    text-align: center;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    margin: 0rem auto;
}

.burger-image{
    max-width: 100%;
    height: auto;
    border-top-left-radius: 30px;
    border-top-right-radius: 30px;
    border-bottom-left-radius: 0px;
    border-bottom-right-radius: 0px;
    transform: scale(1);
}


.burger-p{
    font-size: 1rem;
    max-width: 100%;
    height: auto;
    line-height: 2;
    display: block;
    text-align: left;
    padding: 1rem;
    margin: 2rem auto;
}


/* medieval container */

.schedule-container{
    width: 100%;
    height: auto;
    background-color: transparent;
    border-bottom-left-radius: 30px;
    border-bottom-right-radius: 30px;
    font-family: 'Raleway', sans-serif;
    text-align: center;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    margin: 5rem 0 5rem 0rem;
}

.schedule-image{
    max-width: 100%;
    height: auto;
    border-top-left-radius: 30px;
    border-top-right-radius: 30px;
    border-bottom-left-radius: 0px;
    border-bottom-right-radius: 0px;
    transform: scale(1);
}

.schedule-p{
    font-size: 1rem;
    max-width: 100%;
    height: auto;
    line-height: 2;
    display: block;
    text-align: left;
    padding: 1rem;
    margin: 3rem auto;
}

.bands-container{
    border: 1px solid white;
    width: 100%;
    height: auto;
    background-color: transparent;
    border-bottom-left-radius: 30px;
    border-bottom-right-radius: 30px;
    font-family: 'Raleway', sans-serif;
    text-align: center;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    margin: 0rem auto;
}

.bands-image{
    max-width: 100%;
    height: auto;
    border-top-left-radius: 30px;
    border-top-right-radius: 30px;
    border-bottom-left-radius: 0px;
    border-bottom-right-radius: 0px;
    transform: scale(1);
}


.bands-p{
    font-size: 1rem;
    max-width: 100%;
    height: auto;
    line-height: 2;
    display: block;
    text-align: left;
    padding: 1rem;
    margin: 0 auto;
}


.tickets-container{
    width: 100%;
    height: auto;
    background-color: transparent;
    border-bottom-left-radius: 30px;
    border-bottom-right-radius: 30px;
    font-family: 'Raleway', sans-serif;
    text-align: center;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    margin: 5rem auto;
}

.tickets-image{
    max-width: 100%;
    height: auto;
    border-top-left-radius: 30px;
    border-top-right-radius: 30px;
    border-bottom-left-radius: 0px;
    border-bottom-right-radius: 0px;
    transform: scale(1);
}


.tickets-p{
    font-size: 1rem;
    max-width: 100%;
    height: auto;
    line-height: 2;
    display: block;
    text-align: left;
    padding: 1rem;
    margin: 2rem auto;
}

.supabase-container{
    width: 100%;
    height: auto;
    background-color: transparent;
    border-bottom-left-radius: 30px;
    border-bottom-right-radius: 30px;
    font-family: 'Raleway', sans-serif;
    text-align: center;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    margin: 5rem 0 5rem 0rem;
}

.supabase-image{
    max-width: 100%;
    height: auto;
    border-top-left-radius: 30px;
    border-top-right-radius: 30px;
    border-bottom-left-radius: 0px;
    border-bottom-right-radius: 0px;
    transform: scale(1);
}

.supabase-p{
    font-size: 1rem;
    max-width: 100%;
    height: auto;
    line-height: 2;
    display: block;
    text-align: left;
    padding: 0 0 2rem 1rem;
    margin: 3rem auto;
}

.process-title{
    writing-mode: horizontal-tb; /* vertical writing mode, right-to-left */
    text-orientation: sideways-right; /* characters are upright */
    font-size: 3rem;
    opacity: 0.3;
    margin: 0 5vw;
    color: white;
}

.process-container{
    width: 90%;
    height: auto;
    background-color: transparent;
    border-bottom-left-radius: 30px;
    border-bottom-right-radius: 30px;
    font-family: 'Raleway', sans-serif;
    text-align: center;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: space-around;
    margin: 5rem auto;
    padding: 1rem;
}

.process-p{
    font-size: 1rem;
    margin: 2rem auto;
    max-width: 90%;
    white-space: normal;
    height: auto;
    line-height: 2;
    text-align: left;
}

.process-one-image{
    max-width: 70%;
    height: auto;
    border-bottom-left-radius: 30px;
    border-bottom-right-radius: 30px;
    margin: 2rem 5rem 0 0;
}

.process-two-image{
    max-width: 70%;
    height: auto;
    border-bottom-left-radius: 30px;
    border-bottom-right-radius: 30px;
    margin: 2rem 0 0 5rem;

}

.process-three-image{
    max-width: 100%;
    height: auto;
    border-bottom-left-radius: 30px;
    border-bottom-right-radius: 30px;
    margin: 2rem 0rem 0rem 3rem;
}


/* LAST SECTION */

.last-section{
    height: auto;
    width: 80%;
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: space-around;
    margin: 0 auto;
}

.see-website{
    transform: scale(2);
}

.github-link{
    transform: scale(0.3);
}

.back-to-projects{
    transform: scale(2);
}
}


</style>