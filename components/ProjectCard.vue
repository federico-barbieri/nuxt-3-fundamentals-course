<template>
    <div class="project-card">

        <div class="img-container">
            
               <img :src="img" alt="hola"> 
            
        </div>

        <div class="text-side">

            <h3>{{ name }}</h3>

            <ul class="image-list">
                <li v-for="icon in stack" :key="icon">
                    <img :src="icon" :alt="icon" class="stack-icon" />
                 </li>
            </ul>
      
    
            <p class="description-p">{{ description }}</p>

            <Button class="btnnn" text="See project" />

            

        </div>
       
       

    </div>
</template>

<script setup>

import Button from './Button.vue';


const props = defineProps({
    name: String,
    description: String,
    img: String,
    stack: Array,
});




</script>

<style scoped>

.btnnn{
    height: 3rem;
    margin: 2rem auto;
}



.project-card{
    width: 60vw;
    height: auto;
    color: black;
    transition: all 0.5s ease-in;
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: space-between;
    color: white;
}


h3{
    font-size: 2rem;
    margin-bottom: 2rem;
}



.img-container{
    width: 40%;
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
    width: 50%;
    height: 100%;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: space-around;
    border-top: 1px solid white;
    border-right: 1px solid white;
    padding: 2rem 2rem 0 0;
}

.image-list {
  list-style: none;
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
  gap: 16px;
  width: 100%;
  place-items: center;
}

.stack-icon{
    width: 5rem;
    height: auto;
    filter: drop-shadow(5px 5px 3px var(--dark-slate));
    transition: all 0.5s ease-in;
}

.stack-icon:hover{
  transform: scale(1.1);
}

.description-p{
    font-size: 1rem;
    height: 20%;
}

</style>