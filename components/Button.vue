<template>
    <button>{{ text }}</button>
</template>

<script setup>

const props = defineProps({
  text: String, 
});

</script>

<style scoped>

button{
    border: 1px solid white;
    background-color: transparent;
    color: white;
    font-family: "Poppins", sans-serif;
    width: 10rem;
    height: 5rem;
    transition: all 0.5s ease-in;
}

button:hover{
background-color: white;
color: black;
cursor: pointer;
border-radius: 5px;
filter: drop-shadow(5px 5px 5px black);
}

</style>