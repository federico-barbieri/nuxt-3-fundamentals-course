<template>
    <div class="container">
                
        <video
            class="mondrian"
            ref="loopingVideo"
            autoplay
            muted
            loop
            style="max-width: 100%;"
        >
        <source src="/random/mondrian-2.webm" type="video/webm">
  </video>

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
    width: 30rem;
    height: 15rem;
    background-color: rgb(74,64,44);
    border-bottom-left-radius: 30px;
    border-bottom-right-radius: 30px;
    font-family: 'Raleway', sans-serif;
    color: black;
    text-align: center;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    margin-right: 5rem;
}

.mondrian{
    max-width:100%;
    height: auto;
    border-bottom-left-radius: 30px;
    border-bottom-right-radius: 30px;
}

</style>