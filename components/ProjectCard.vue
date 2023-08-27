<template>
    <div class="project-card">

        <div>
            <div>
                <img :src="img" alt="">
            </div>
        </div>

        <div class="text-side">

            <h3>{{ name }}</h3>
      
    
            <p>{{ description }}</p>

            <div class="project-code">
            
            </div>

        </div>
       
       

    </div>
</template>

<script setup>


const props = defineProps({
  name: String,
  description: String,
  img: String 
});



</script>

<style scoped>

.project-card{
    width: 100%;
    height: 30rem;
    border: 2px solid red;
    color: white;
}

h3{
    font-size: 2rem;
}

</style>