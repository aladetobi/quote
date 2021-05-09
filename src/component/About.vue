<template>
    <section class="about">
        <div class="container">
            <div class="first">
                    <div class="text-line">
                        <h3 class="heading-3"><span>01.</span>About</h3>
                    </div>
                    <p class="paragraph">
                        Hello! My name is Tobi and i enjoy creating things that live on the internet. 
                        My internet in web development started in 2018 when i decided to try editing custom Tumbir themes - turns out
                        hacking together a custom reblog button taught me a lot about HTML & CSS!
                    </p>
                    <p class="paragraph">
                        Fast-forward to today, and i've had the privilege of working at 
                        <span>an advertising agency, a start-up, a huge corporation, and 
                            a student-led design studio.</span> My main focus these days is building 
                            accessible, inclusive products and digital experiences at 
                            <span>Upstatement</span> for a variety of clients.
                    </p>
                    <p class="paragraph">Here are a few technologies I've been working with recently:</p>
                    <ul class="section__list">
                        <li class="section__list-item"><span></span> Javascript (ES6+)</li>
                        <li class="section__list-item">css</li>
                        <li class="section__list-item">Bootstrap</li>
                        <li class="section__list-item">VueJs</li>
                        <li class="section__list-item">sass</li>
                        <li class="section__list-item">Node.js</li>
                    </ul>    
            </div>
            <div class="about__photo">
                <div class="about__image">
                    <img src="../assets/profile.jpg" alt="" class="about__image-img">
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
    .about {
        width: 100%;
        background-color: rgba(0, 0, 0, 0.99);
        color: #ddd;
    }
    .container {
        width: 100rem;
        margin: 0 auto;
        padding: 15rem 0;
        display: flex;
        align-items: center;
        justify-content: center;
        
    }

   .text-line {
       display: flex;
       align-items: center;
       justify-content: center;
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

     .paragraph {
        font-size: 1.3rem;
        width: 40rem;
        margin: 3rem 0;
    }

    .first p.paragraph:nth-child(4) {
        margin: 1rem auto;
    }
    .paragraph span {
        color: #69F7C1;
    }

    .section__list {
        list-style-type: square;
        list-style-position: inside;
        list-style-image: linear-gradient(to right, #69f7c1, #69f7c1);
        width: 70%;
        margin: 0 auto;
        display: flex;
        flex-wrap: wrap;
        justify-content: center;
    }

    .section__list-item {
        flex: 40%;
        font-size: 1.5rem;
    }


    .about__photo {
        margin-left: 7rem;
    }
    .about__image {
       width: 30rem;
       height: 30rem;
       border-radius: 1rem; 
       position: relative;
       z-index: 2;
    }

    .about__image::after {
        content: '';
        position: absolute;
        top: 3rem;
        right: -3rem;
        height: 100%;
        width: 100%;
        border-radius: 1rem;
        border: .5rem solid #69f7c1;
        z-index: -2;
    }

    .about__image-img {
        width: 100%;
        object-fit: cover;
        border-radius: 1rem;
        border: .5rem solid black;
        filter: brightness(60%);
    }

    @media screen and (max-width: 56.25em) {
        .container {
            padding: 10rem 0 15rem 0;
            width: 100%;
            flex-direction: column;
            font-size: 3rem;
        }
    
        .first {
            flex: 50rem;
        }
        .paragraph {
            width: 80%;
            margin: 3rem auto;
        }
        .about__photo {
            margin-left: 0;
        }
        
        .about__image {
            width: 40rem;
            height: 30rem;
        }
        /* .about__image::after {
        content: '';
        position: absolute;
        top: 0;
        right: 0;
        height: 110%;
        width: 110%;
        border-radius: 1rem;
        border: .5rem solid #69f7c1;
        z-index: 12;
    } */
    }
</style>