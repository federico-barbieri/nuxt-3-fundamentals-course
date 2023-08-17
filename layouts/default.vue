<template>
    <div>
    <header>
        <nav>
            <span>LOGO HERE</span>
            <ul>
                <li>ABOUT</li>
                <li>PROJECTS</li>
            </ul>
        </nav>
    </header>
    <slot />
    <footer>
        <p>I am a footer, respect me</p>
    </footer>
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


header{
    width: 100vw;
    height: 15vh;
    background-color: var(--primary-blue);
    background-color: var(--dark-slate);
    color: var(--near-white);
}

nav{
    width: 100%;
    height: 100%;
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: space-around;
}

nav > ul{
    width: 50%;
    height: 100%;
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: space-around;
    list-style-type: none;
}

footer{
    width: 100vw;
    height: 15vh;
    background-color: var(--primary-blue);
    background-color: var(--dark-slate);
    color: var(--near-white);
    display: flex;
    align-items: center;
    justify-content: center;
}

</style>