<template>
    <div class="project-card">
       
        <h3>{{ name }}</h3>
      
    
        <p>{{ description }}</p>

    </div>
</template>

<script setup>


const props = defineProps({
  name: String,
  description: String
});

</script>

<style scoped>

.project-card{
    width: 15rem;
    height: 15rem;
    border: 2px solid red;
    color: white;
}

h3{
    font-size: 2rem;
}

</style>