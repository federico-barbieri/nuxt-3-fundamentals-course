<template>
    <div>
    <header>
        <nav>
            <span><nuxt-link to="/">LOGO</nuxt-link></span>
            <ul>
                <li><nuxt-link to="https://www.linkedin.com/in/fedebarbieri/" target="_blank"><img class="linkedin" src="/icons/linkedin.png" alt=""></nuxt-link></li>
                <li><nuxt-link to="https://github.com/federico-barbieri" target="_blank"><img src="/icons/github.png" alt=""></nuxt-link></li>
            </ul>
        </nav>
    </header>
    <slot />
   
    </div>  
</template>

<script>
export default {
    setup () {
        

        return {}
    }
}
</script>

<style scoped>

a{
    color: inherit;
    text-decoration: none;
}

a:visited{
    color: inherit;
    text-decoration: none;
}


header{
    width: 100vw;
    height: 15vh;
    background-color: var(--primary-blue);
    background-color: rgb(17,17,17);
    color: var(--near-white);
    font-family: "Roboto", sans-serif;
}

nav{
    width: 100%;
    height: 100%;
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: space-between;
    font-size: 1.5rem;
}

nav > ul{
    width: 40%;
    height: 80%;
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: center;
    list-style-type: none;
    border: 1px solid white;
}

ul > li {
    transition: all 0.5s ease-in;
    transform: scale(0.2);
}

.linkedin{
    transform: scale(0.7);
}

ul > li:hover {
    transition: all 0.5s ease-in;
    text-decoration: underline;
}

</style>