<template>
    <div>
        I AM THE PROJECTS PAGE

        <nuxt-link to="/"> bacvk to index</nuxt-link>

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

    </div>
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