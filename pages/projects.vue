<template>

<main>


    <section class="hero">

        <h1>PROJECTS</h1>
     
                    
                    <div class="project-cards">
                        <ProjectCard class="messiverse"  name="Messiverse" description="A multiverse of Messis" img="/projectImgs/messi.png"  />
                        <ProjectCard class="hackers" name="Magic Hackers"  description="A dashboard for Dumbledore" img="/projectImgs/hogwarts.png" />
                        <ProjectCard class="sakurai" name="Jimmy Sakurai" description="A tribute to a great guitar player" img="/projectImgs/moon.png" />
                        <ProjectCard class="swampfest" name="SwampFest"  description="The best festival in the world" img="/projectImgs/shrek.jpg" />
                    </div>
                    
                    

</section>





<section class="contact">
    <h2 class="contact-title">CONTACT</h2>
    <p>let's get in touch!</p>
</section>




</main>

    
</template>

<script setup>

const kea = ref(false);

function toggleKea(){
    kea.value = true;
    if(personal.value){
        personal.value = false;
    }
}

const personal = ref(false);

function togglePersonal(){
    personal.value = true;
    if(kea.value){
        kea.value = false;
    }
}

const allProjects = ref(false);

function toggleAll(){
    kea.value = true;
    personal.value = true;
}

</script>

<style scoped>

.toggle-btns-project-page{
    width: 8rem;
    height: 3rem;
    border-radius: 5px;
}


.messiverse{
    background-color: black;
}

.hackers{
    background-color: hotpink;
}

.sakurai{
    background-color: aqua;
}

.swampfest{
    background-color: saddlebrown;
}

.bikini{
    background-color: yellow;
}

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
    height: auto;
    width: 100vw;
}

h1{
    font-size: 15rem;
    opacity: 0.3;
    text-align: center;
}

h2{
    font-size: 15rem;
    opacity: 0.3;
}

.project-cards{
    width:100%;
    height: auto;
    margin: 0 auto;
    display: flex;
    flex-direction: column;
    align-items: center;
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