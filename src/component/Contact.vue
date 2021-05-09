<template>
<footer class="footer">
    <div class="container">
        <h4>Follow me up</h4>
        <div class="text-line">
            <h3 class="heading-3"><span>04. What's Next?</span></h3>
        </div>
        <h1 class="heading">Get In touch</h1>
        <p>Although I'm not currently looking for any new opportunities, my inbox is always open. 
            Whether you have a question or ust want to say hi, I'll try my best to get back to you!
        </p>
        <btn class="btn">Say Hello</btn>
    </div>
</footer>
</template>

<script>
    export default {
       
    }
</script>

<style scoped>

    .footer {
        background-color: rgba(0, 0, 0, .99);
        color: #ddd;
    }

    .container {
        width: 100rem;
        min-height: 100vh;
        margin: 0 auto;
        text-align: center;
        padding: 5rem 0 10rem 0;
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
    }
    .text-line {
       display: flex;
       align-items: center;
       height: 2rem;
    }

    .heading-3 {    
        font-size: 2rem;
        line-height: 1;
    }

    .heading-3 span {
        color: #69F7C1;
        font-size: 1.7rem;
    }

    .heading {
        font-size: 4rem;
        margin: 2rem 0;
    }

    h4 {
        padding: .5rem;
        margin-bottom: 3rem;
        letter-spacing:.5rem;
        background-color: #111;
    }

    p {
        font-size: 1.2rem;
        width: 40rem;
        margin-top: 2rem;
    }
    .btn {
        margin-top: 3rem;
    }
</style>