<template>
    <div>
       <header class="header">
           <div class="container">
                <h3 class="header__heading-3">Hi, my name is</h3>
                <h1 class="header__heading-1">Alade Tobi.</h1>
                <h2 class="header__heading-2">I build things for the web.</h2>
                <p class="paragraph">
                I'm a Lagos-based front-end engineer who specializes in building 
                (and occasionally designing) exceptional digital experiences. 
                Currently, I'm an engineer at <a href="">Upstatement</a> focused on buiding 
                accessible, human-centered products.
                </p>
                <button href="" class="btn header__btn">Get In Touch</button>
            </div>
       </header>
    </div>
</template>

<script>
    export default {
        
    }
</script>

<style scoped>
    .header {
        background-color: rgba(0, 0, 0, 0.99);
        color: #ddd;
        height: calc(100vh - 6rem);
        width: 100%;
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: flex-end;
    }
    .container {
        width: 100rem;
        margin: 0 auto;
    }

    .header__heading-3 {
        color: #69F7C1;
        font-size: 1.4rem;
        line-height: 1;
        margin-bottom: 1rem;
    }

    .header__heading-1 {
        font-size: 7rem;
        letter-spacing: .5rem;
        color: #fff;
        line-height: 1;
    }

    .header__heading-2 {
        font-size: 5rem;
        letter-spacing: 2px;
    }

    .paragraph {
        font-size: 1.3rem;
        width: 40rem;
        margin: 3rem 0;
    }

    .paragraph a {
        color: #69F7C1;
        text-decoration: none;
    }

    .header__btn {
        border-radius: 2px;
    }

    @media screen and (max-width: 68.75em) {
        .container {
            width: 80rem;
        }
    }
    @media screen and (max-width: 56.25em) {
        .header {
            height: 100vh;
        }
    }
    @media screen and (max-width: 50em) {
        .container {
            padding-right: 7rem;
            padding-left: 7rem;
        }
    }
    
</style>