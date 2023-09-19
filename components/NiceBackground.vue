<template>
    <div class="container">

        <img class="background" src="/random/nice-background.webp" alt="">
            

    </div>
</template>

<script setup>

import { ref, onMounted } from 'vue';

const loopingVideo = ref(null);

onMounted(() => {
      // Access the video element and play it
      loopingVideo.value.play();
    });


</script>

<style scoped>

.container{
    max-width: 70rem;
    height: auto;
    background-color: rgb(74,64,44);
    border-bottom-left-radius: 30px;
    border-top-right-radius: 30px;

    font-family: 'Raleway', sans-serif;
    color: black;
    text-align: center;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    margin: 0 10vw;
}

.background{
    max-width: 100%;
    height: auto;
    border-bottom-left-radius: 30px;
    border-top-right-radius: 30px;

}

</style>