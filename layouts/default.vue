<template>
    <div>
    <header>
        <nav>
            <div class="logo">
            <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-arrow-right arrow-logo" viewBox="0 0 16 16">
              <path fill-rule="evenodd" d="M1 8a.5.5 0 0 1 .5-.5h11.793l-3.147-3.146a.5.5 0 0 1 .708-.708l4 4a.5.5 0 0 1 0 .708l-4 4a.5.5 0 0 1-.708-.708L13.293 8.5H1.5A.5.5 0 0 1 1 8z"/>
            </svg>
            <span class="f"><nuxt-link to="/">FB</nuxt-link></span>
            </div>
            <ul>
                <li><nuxt-link to="https://www.linkedin.com/in/fedebarbieri/" target="_blank"><img class="linkedin" src="/icons/linkedin.png" alt="LinkedIn logo"></nuxt-link></li>
                <li><nuxt-link to="https://github.com/federico-barbieri" target="_blank"><img class="github" src="/icons/github.png" alt="Github logo"></nuxt-link></li>
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

nav > .logo{
    width: 20%;
}

nav > ul{
    width: 40%;
    height: 80%;
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: center;
    list-style-type: none;
}

ul > li {
    transition: all 0.5s ease-in;
    transform: scale(0.2);
}



.linkedin{
    transform: scale(0.7);
    transition: all 0.5s ease-in
}

.linkedin:hover{
    transform: scale(0.8);
}

.github{
    transform: scale(1);
    transition: all 0.5s ease-in
}

.github:hover{
    transform: scale(1.1);
}

ul > li:hover {
    transition: all 0.5s ease-in;
    text-decoration: underline;
}

.logo{
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: center;
}

.arrow-logo{
    transform: scale(3);
    opacity: 0;
    transition: all 0.5s;
}

.logo:hover .arrow-logo{
        opacity: 1;
        margin: 0 0 0 4rem;
        transform: scale(3), translateX(2rem);
}

.logo:hover .f{
    font-size: 3.5rem;
    font-family: 'Exo', sans-serif;
    writing-mode: vertical-lr; /* vertical writing mode, right-to-left */
    transform: translateX(2rem);
}



.f{
    font-size: 3.5rem;
    font-family: 'Exo', sans-serif;
    writing-mode: vertical-lr; /* vertical writing mode, right-to-left */
    transition: all 0.5s ease-in;
}


@media screen and (max-width: 767px) {
  
nav > ul{
    width: 20%;
    height: 80%;
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: center;
    list-style-type: none;
    display: none;
}

nav > .logo{
    width: 100%;
}




}


</style>