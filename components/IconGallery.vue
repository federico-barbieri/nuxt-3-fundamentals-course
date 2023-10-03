<template>
    <ul class="image-list">
    <li v-for="(image, index) in images" :key="index">
      <img data-tooltip="image.name" :src="image.path" :alt="image.name" class="stack-icon" />
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
  margin: 0 auto;
  place-content: center;
  gap: 0px;
}

ul{
  padding-inline-start: 0;
}

.stack-icon{
    max-width: 5rem;
    height: auto;
    filter: drop-shadow(10px 10px 3px var(--dark-slate));
    transition: all 0.5s ease-in;
}

.stack-icon:hover{
  transform: scale(1.1);
}

/* Tablet Styles */
@media screen and (min-width: 768px) and (max-width: 1300px) {
  .image-list{
    margin: 0 auto;
    place-items: center;
    gap: 0px;

    list-style: none;
  display: grid;
  grid-template-columns: 1fr 1fr 1fr 1fr 1fr;
  gap: 0;
  margin: 0 auto;
  place-content: center;
  gap: 0px;
  }
}

@media screen and (max-width: 767px) {
  .image-list{
    margin: 0 auto;
    place-items: center;
    gap: 0px;
    width: 100%;
    grid-template-columns: 1fr 1fr 1fr 1fr 1fr;

  }
  .stack-icon{
    max-width: 4rem;
    height: auto;
    filter: drop-shadow(10px 10px 3px var(--dark-slate));
    transition: all 0.5s ease-in;
}

}


</style>