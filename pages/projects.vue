<template>
    <div>
        I AM THE PROJECTS PAGE

        <nuxt-link to="/"> bacvk to index</nuxt-link>

        <ul class="project-list">

                    <button @click="toggleKea">KEA</button>
                    <button @click="togglePersonal">PERSONAL PROJECTS</button>
                    
                    <ProjectCard class="messiverse" v-if="kea" name="Messiverse" description="a cool project" img="/images/hogwarts.png" />
                    <ProjectCard name="Magic Hackers" v-if="kea" description="a cool project" img="" />
                    <ProjectCard name="Jimmy Sakurai" v-if="personal" description="a cool project" img="" />
                    <ProjectCard name="SwampFest" v-if="kea" description="a cool project" img="" />

                    
                    </ul>

    </div>
</template>

<script setup>

const kea = ref(false);

function toggleKea(){
    kea.value = !kea.value;
}

const personal = ref(false);

function togglePersonal(){
    personal.value = !personal.value;
}

</script>

<style scoped>

.messiverse{
    background-color: black;
}

</style>