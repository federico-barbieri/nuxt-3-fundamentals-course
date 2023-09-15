<template>

<main>

<section class="hero">

    <section>
     

        <ul class="project-list">

                    <button @click="toggleKea">KEA</button>
                    <button @click="togglePersonal">PERSONAL PROJECTS</button>
                    <button @click="toggleAll">ALL PROJECTS</button>
                    
                    <ProjectCard class="messiverse" v-if="kea" name="Messiverse" description="A multiverse of Messis" img="/images/hogwarts.png" />
                    <ProjectCard class="hackers" name="Magic Hackers" v-if="kea" description="A dashboard for Dumbledore" img="" />
                    <ProjectCard class="sakurai" name="Jimmy Sakurai" v-if="personal" description="A tribute to a great guitar player" img="" />
                    <ProjectCard class="swampfest" name="SwampFest" v-if="kea" description="The best festival in the world" img="" />
                    <ProjectCard class="bikini" name="CPH Cartel" v-if="kea" description="An immersive experience" img="" />

                    
                    </ul>

    </section>

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
        <ProjectCard name="Magic Hackers" description="A dashboard for Dumbledore" img="/projectImgs/hogwarts.png" />
        <ProjectCard name="Jimmy Sakurai" description="A tribute to a great guitar player" img="/projectImgs/moon.png" />
        <ProjectCard name="SwampFest" description="The best festival in the world" img="/projectImgs/shrek.jpg" />

        
        </ul>



    </div>
    
   
    <h2 class="projects-title"> <nuxt-link to="/projects">PROJECTS</nuxt-link></h2>
    
</section>

<section class="stack">

    <h2 class="stack-title"> <nuxt-link to="/projects">STACK</nuxt-link></h2>

    <div class="p-and-ul">

        <p class="stack-p">Over the years, I've become more and more comfortable with different technologies.</p>

        <IconGallery :images="stackArray" />
        
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

</style>