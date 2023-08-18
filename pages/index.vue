<template>
    <div>

        <main>

            <section class="hero">

                <h1><span class="federico">FEDERICO</span> <span class="barbieri">BARBIERI</span></h1>
                <span class="frontend-developer">FRONTEND DEVELOPER</span>

            </section>

            <section class="about">

                <h2 class="about-title">ABOUT</h2>
                <p class="about-p">Student, bla bla, background, internship, tools and technologies</p>

            </section>

            <section class="projects">
                <h2 class="projects-title">PROJECTS</h2>
                <p>Check a selection of projects I've been working on over the past year</p>
            </section>

            <section class="contact">
                <h2 class="contact-title">CONTACT</h2>
                <p>let's get in touch!</p>
            </section>

            


        </main>

</div>
</template>

<script setup>

</script>

<style scoped>

/* MAIN */

main{
    width: 100vw;
    height: auto;
    color: var(--near-white);
    display: flex;
    flex-direction: column;
    font-family: "Poppins", sans-serif;
    background-color: var(--neutral-gray);
    overflow: hidden;
}

/* HERO */

.hero{
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    height: 85vh;
    width: 100vw;

}

h1{
    font-size: 5rem;
    text-align: center;
}

.federico{
    text-decoration: underline;
    display: inline-block;
    transform: translate(3rem, -5.39rem);
}

.barbieri{
    text-decoration: overline;
    display: inline-block;
    transform: translate(1.5rem, 0.61rem);
}

.frontend-developer{
    font-size: 1.5rem;
}

h2{
    font-size: 18rem;
}

/* ABOUT */

.about{
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: center;
    height: 85vh;
    width: 100%;
}

.about-title{
    text-decoration: overline;
}

.about-p{
    font-size: 1.5rem;
    margin-left: 2rem;
}




/* PROJECTS */

.projects{
    display: flex;
    flex-direction: column;
    align-items: flex-end;
    justify-content: center;
    height: 85vh;
    width: 100%;
}

.projects-title{
    text-decoration: underline;
}

/* CONTACT */

.contact{
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: center;
    height: 85vh;
    width: 100%;
}

.contact-title{
    text-decoration: overline;
}

</style>