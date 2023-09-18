<template>

<main>


    <section class="hero">

        <h1>PROJECTS</h1>
     
                    
                    <div class="project-cards">
                        <ProjectCard 
                        class="messiverse"  
                        name="Messiverse" 
                        description="A multiverse of Messis" 
                        img="/projectImgs/messi.png"
                        :stack="['/icons/vuejs.png', '/icons/vitejs.png', '/icons/openai.png']"
                        />

                        <ProjectCard 
                        class="swampfest" 
                        name="SwampFest"  
                        description="The best festival in the world" 
                        img="/projectImgs/shrek.jpg"
                        :stack="['/icons/nextjs2.png', '/icons/git.png', '/icons/typescript.png']"
                        />

                        <ProjectCard 
                        class="hackers" 
                        name="Magic Hackers"  
                        description="A dashboard for Dumbledore" 
                        img="/projectImgs/hogwarts.png"
                        :stack="['/icons/ai.svg', '/icons/ps.svg', '/icons/js.svg']"
                        />

                        <ProjectCard 
                        class="edc" 
                        name="EDC"  
                        description="Find the house of your dreams" 
                        img="/projectImgs/ecd.jpg"
                        :stack="['/icons/xd.svg', '/icons/figma.svg', '/icons/reactjs.svg']"
                        />
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
   margin-bottom: 5rem;
}

.hackers{
    margin-bottom: 5rem;

}

.sakurai{
    margin-bottom: 5rem;

}

.swampfest{
    margin-bottom: 5rem;

}

.bikini{
    margin-bottom: 5rem;

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
    width: 100%;
    height: auto;
    margin: 0 auto;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: space-around;
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