<template>
    <section class="project">
        <div class="container">
            <div class="text-line mb">
                <h3 class="heading-3"><span>03.</span>Something i've built</h3>
            </div>
            <div class="built">
                <div class="built__img built__img--one">
                    <img src="../assets/profile.jpg" alt="" class="built__img--img">
                </div>
                <div class="built__text built__text--one">
                    <span>Featured Project</span>
                    <h3>OctoProfile</h3>
                    <p>
                        A nicer look at your Github profile and repository stat with data visualizations of your top languages and stars. Sort through your top repos by number of stars, forks and size.
                    </p>
                    <pre>Nex.js Chart.js Github API</pre>
                    <span>&larr;   &rarr;</span>
                </div>
            </div>
            <div class="built">
                <div class="built__text built__text--two">
                    <span>Featured Project</span>
                    <h3>OctoProfile</h3>
                    <p>
                        A nicer look at your Github profile and repository stat with data visualizations of your top languages and stars. Sort through your top repos by number of stars, forks and size.
                    </p>
                    <pre>Nex.js Chart.js Github API</pre>
                    <span class="icon">&larr;   &rarr;</span>
                </div>
                <div class="built__img built__img--two">
                    <img src="../assets/profile.jpg" alt="" class="built__img--img">
                </div>
            </div>
            <div class="built">
                <div class="built__img built__img--one">
                    <img src="../assets/profile.jpg" alt="" class="built__img--img">
                </div>
                <div class="built__text built__text--one">
                    <span>Featured Project</span>
                    <h3>OctoProfile</h3>
                    <p>
                        A nicer look at your Github profile and repository stat with data visualizations of your top languages and stars. Sort through your top repos by number of stars, forks and size.
                    </p>
                    <pre>Nex.js Chart.js Github API</pre>
                    <span>&larr;   &rarr;</span>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
    export default {       
    }
</script>

<style scoped>


    .mb {
        margin-bottom: 6rem;
    }


   .project {
        width: 100%;
        background-color: rgba(0, 0, 0, 0.99);
        color: #ddd;
    }
    .container {
    width: 100rem;
    margin: 0 auto;
    padding: 15rem 0;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    }

    .text-line {
        /* align-self: flex-start; */
       display: flex;
       align-items: center;
       height: 2rem;
    }

   .text-line::after {
       display: block;
       content: '';
       width: 30rem;
       height: .01rem;
       margin-left: 1rem;
       background-color: #eee;
    }

    .heading-3 {    
        font-size: 2rem;
        line-height: 1;
    }

    .heading-3 span {
        color: #69F7C1;
        margin-right: 1rem;
        font-size: 1.7rem;
    }

    .built {
        display: flex;
        justify-content: center;
        align-items: center;
        margin-bottom: 10rem;
    }

    .built:last-child {
        margin-bottom: 0;
    }

    .built__img {
        flex: 70%;
        height: 40rem;
    }

    .built__img--img {
        height: 100%;
        width: 60rem;
        object-fit: cover;
        filter: brightness(60%);
        box-shadow: .1rem .1px 2rem #333;
        transition: filter .3s;
    }

    .built__img--img:hover {
        filter: brightness(90%);
    }

    .built__text {
        flex: 30%;
        text-align: right;
        margin-left: -30rem;
        font-size: 1rem;
        z-index: 1;
    }

    .built__text span {
        /* text-align: left; */
        display: block;
        color: #69F7C1;
        font-size: 1.1rem;
    }

    .built__text h3 {
        font-size: 1.8rem;
    }

    .built__text p {
        display: inline-block;
        font-size: 1.2rem;
        margin: 2rem 0;
        background-color: #111;
        padding: 2rem;
        padding-left: 3rem;
        box-shadow: .1rem .1px .5rem #333;
    }

    .built__text .icon {
        font-size: 1.5rem;
    }

    .built__text--two {
        text-align: left;
        margin-left: 0;
        margin-right: 0;
        flex: 50%;
        margin-right: -30rem;
    }

    .built__text--two p {
        margin: 2rem 0;
        padding: 2rem;
        display: block;
    }

    .built__img--two {
        margin-left: 40rem; 
    }

    @media screen and (max-width: 68.75em) {
        .built__img {
        flex: 70%;
        height: 40rem;
    }

        .built__img--img {
            height: 100%;
            width: 40rem;
            object-fit: cover;
            filter: brightness(60%);
            box-shadow: .1rem .1px 2rem #333;
            transition: filter .3s;
        }
    }

</style>