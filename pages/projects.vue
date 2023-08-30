<template>
    <div>
        I AM THE PROJECTS PAGE

        <nuxt-link to="/"> bacvk to index</nuxt-link>

        <ul class="project-list">
                    
                    <ProjectCard name="Messiverse" description="a cool project" img="/images/hogwarts.png" />
                    <ProjectCard name="Magic Hackers" description="a cool project" img="" />
                    <ProjectCard name="Jimmy Sakurai" description="a cool project" img="" />
                    <ProjectCard name="SwampFest" description="a cool project" img="" />

                    
                    </ul>

    </div>
</template>

<script>
export default {
    setup () {
        

        return {}
    }
}
</script>

<style scoped>

</style>