<template>
    <div class="container">

        <img class="dog" src="/random/run.gif" alt="">
            

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
    width: 20rem;
    height: 15rem;
    background-color: rgb(74,64,44);
    font-family: 'Raleway', sans-serif;
    color: black;
    text-align: center;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    margin-top: 2rem;
}

.dog{
    max-width: 100%;
    height: auto;
    border-bottom-left-radius: 30px;
}

</style>