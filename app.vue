<template>
    <div>
        <NuxtLayout>
        <nuxtPage />
        </NuxtLayout>
    
    </div>
</template>

<script>
export default {
    setup () {
        

        return {}
    }
}
</script>

<style>

*{
    margin: 0;
    box-sizing: border-box;
}


.page-enter-active,
.page-leave-active {
  transition: all 0.4s;
}
.page-enter-from,
.page-leave-to {
  opacity: 0;
  filter: blur(1rem);
}

</style>