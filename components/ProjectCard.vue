<template>
    <div class="project-card">

        <div class="img-container">
            
               <img :src="img" alt="hola"> 
            
        </div>

        <div class="text-side">

            <h3>{{ name }}</h3>
      
    
            <p>{{ description }}</p>

            

        </div>
       
       

    </div>
</template>

<script setup>


const props = defineProps({
    name: String,
    description: String,
    img: String,
});




</script>

<style scoped>



.project-card{
    max-width: 80%;
    min-width: 50%;
    height: 15rem;
    color: black;
    transition: all 0.5s ease-in;
    display: flex;
    flex-direction: row;
    color: white;
    border-right: 1px solid rgba(255, 255, 255, 0.3);
    transition: all 1s ease-in;
}

.project-card:hover{
    max-width: 80%;
    min-width: 50%;
    height: 18rem;
    color: black;
    transition: all 0.5s ease-in;
    display: flex;
    flex-direction: row;
    color: white;
    border: 1px solid rgba(255, 255, 255, 0.3);
}

.project-card:hover h3{
    font-size: 3rem;
}

h3{
    font-size: 2rem;
    transition: all 0.5s ease-in;

}



.img-container{
    width: 50%;
    height: 100%;
    overflow: hidden;
    filter: drop-shadow(5px 5px 5px black);

}

img{
    max-width: 100%;
    height: auto;
    border-radius: 10px;

}

.text-side{
    width:50%;
    height: 100%;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: space-around;
}

</style>