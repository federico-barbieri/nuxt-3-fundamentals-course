<template>
    <div class="project-card" :style="{ 'margin': margin}" @mouseover="handleMouseOver" @mouseout="handleMouseOut">

        

        <div class="text-side" :style="{ 'border-top': border_top, 'border-bottom': border_bottom}">

            <h3 v-show="!isBeingHovered">{{ name }}</h3>

            <ul class="image-list" v-show="!isBeingHovered">
                <li v-for="icon in stack" :key="icon">
                    <img :src="icon" :alt="icon" class="stack-icon" />
                 </li>
            </ul>
      
    
            <p v-show="!isBeingHovered" class="description-p" v-html="description"></p>

            <nuxt-link v-show="isBeingHovered" :to="liveProject"><Button class="btnnn" text="See project"></Button></nuxt-link>

            

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
    border_bottom: String,
    border_top: String,
    margin: String,
    liveProject: String,
});

let isBeingHovered = ref(false);

// Method to handle mouseover event
const handleMouseOver = () => {
      isBeingHovered.value = true;
    };

    // Method to handle mouseout event
    const handleMouseOut = () => {
      isBeingHovered.value = false;
    };



</script>

<style scoped>

.text-side:hover h3,
.text-side:hover .image-list,
.text-side:hover .description-p {
  visibility: hidden;
}

.btnnn{
    height: 3rem;
    margin: 2rem auto;
}



.project-card{
    width: 50rem;
    height: 30rem;
    color: black;
    transition: all 0.5s ease-in;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: space-between;
    color: white;
    margin-right: 5rem;
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
    width: 100%;
    height: 100%;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: space-around;
    padding: 2rem 2rem 0 0;
    word-wrap: break-word;
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
    height: 30%;
    width: 100%;
    line-height: 2;
    text-align: center;
}


@media screen and (max-width: 767px) {
    .text-side:hover h3,
.text-side:hover .image-list,
.text-side:hover .description-p {
  visibility: visible;
}
    .btnnn{
    height: 3rem;
    margin: 2rem auto;
}



.project-card{
    width: 95%;
    height: auto;
    color: black;
    transition: all 0.5s ease-in;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: space-between;
    color: white;
    margin: 2rem auto 0 auto !important;
    border: 2px solid red;
}


h3{
    font-size: 2rem;
    margin-bottom: 2rem;
}



.img-container{
    width: 100%;
    height: auto;
    overflow: hidden;
    filter: drop-shadow(5px 5px 5px black);
    margin: 0 auto 0 auto;
}

img{
    max-width: 100%;
    height: auto;
    border-radius: 10px;

}

.text-side{
    width: 100%;
    height: auto;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: space-around;
    padding: 2rem;
    word-wrap: break-word;
}

.image-list {
  list-style: none;
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
  gap: 0;
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
    height: auto;
    width: 100%;
    line-height: 2;
    text-align: center;
}
}


</style>