<template>
    <div>

        <main>

            <!-- HERO SECTION -->

            <section class="hero">

                <!-- TITLE CONTAINER -->

                <div class="title-container">

                    <div class="title-inner-div">
                        <h1><span class="federico">ADVERTISING</span></h1>

                    </div>

                    <a :href="`#${scrollToElementId}`">
                        <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-arrow-right arrow-name" viewBox="0 0 16 16">
                            <path fill-rule="evenodd" d="M1 8a.5.5 0 0 1 .5-.5h11.793l-3.147-3.146a.5.5 0 0 1 .708-.708l4 4a.5.5 0 0 1 0 .708l-4 4a.5.5 0 0 1-.708-.708L13.293 8.5H1.5A.5.5 0 0 1 1 8z"/>
                        </svg>
                    </a>


                </div>

                <!-- BURGER MENU CONTAINER -->


                <div class="burger-container" :id="scrollToElementId">
        
                    <img class="burger-image" src="/advertising/run.gif" alt="Gif of a running dog">
                    
                    <p>
                    After a decade of experience working with international brands,<br>
                    there is one thing I'm certain: <br><br>
                    <i>It's not a sprint. It´s a marathon.</i>
                    </p>

                </div>
                
                <!-- SCHEDULE CONTAINER -->

                <div class="schedule-container">

                    <img class="schedule-image" src="/advertising/ad-print.png" alt="Print advertising for Heisenberg and for Volkswagen">

                    <p>
                    No two days are the same. <br>
                    One day can involve coming up with a print ad for an optical shop.<br>
                    Another day can be about a digital campaign for Volkswagen.
                    </p>


                </div>

                <!-- BANDS CONTAINER -->

                <div class="bands-container">

                    <img class="bands-image" src="/advertising/print-horizontal.jpg" alt="Print ads for champagne, cars and wines.">

                    <p>
                    The same can be said about brands.<br>
                    
                    </p>


                </div>

                <!-- TICKETS CONTAINER -->

                <div class="tickets-container">

                    <video class="tickets-image" src="/advertising/commercials-reel.mp4" controls alt="Commercials reel"></video>

                    <p>
                    Check some of the highlights in my career.
                    </p>


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

p{
    font-size: 1.5rem;
    margin: 0rem 0 0 2rem;
    width: 40rem;
    height: 50%;
    line-height: 2;
    text-align: left;
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

/* HERO SECTION */

.hero{
    display: flex;
    flex-direction: row;
    align-items: center;
    height: 85vh;
    width: 500vw;
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
    max-width: 30%;
    height: auto;
    border-bottom-left-radius: 30px;
    border-bottom-right-radius: 30px;
    transform: scale(0.8);
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
    max-width: 60%;
    height: auto;
    border-bottom-left-radius: 30px;
    border-bottom-right-radius: 30px;
    transform: scale(0.8);
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
    width: 250vw;
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

/* LAST SECTION */

.last-section{
    height: 80%;
    display: flex;
    flex-direction: column;
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


</style>