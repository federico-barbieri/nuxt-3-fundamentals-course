<template>
    <div class="container">
                
        <video
            class="cortazar"
            ref="loopingVideo"
            autoplay
            muted
            loop
            style="max-width: 100%;"
        >
        <source src="/random/cortazar.webm" type="video/webm">
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
    width: 15rem;
    max-height: 15rem;
    background-color: rgb(74,64,44);
    border-radius: 30px;
    font-family: 'Raleway', sans-serif;
    color: black;
    text-align: center;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
}

.cortazar{
    max-width:100%;
    height: auto;
    border-radius: 30px;
}

</style>