<template>
    <ul class="image-list">
    <li v-for="(image, index) in images" :key="index">
      <img :src="image.path" :alt="image.name" class="stack-icon" />
    </li>
  </ul>
</template>

<script setup>

const props = defineProps({
      images: Array,
    });

</script>

<style scoped>

.image-list {
  list-style: none;
  display: grid;
  grid-template-columns: 1fr 1fr 1fr 1fr;
  gap: 16px;
}

.stack-icon{
    width: 8rem;
    height: auto;
    filter: drop-shadow(10px 10px 3px var(--dark-slate));
    transition: all 0.5s ease-in;
}

.stack-icon:hover{
  transform: scale(1.1);
}

</style>