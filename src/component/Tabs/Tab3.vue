<template>
    <div>
       <div>
            <h1>UI Engineer Co-op <span>@ Apple</span></h1>
            <p>July - December 2017</p>
            <ul>
                <li>Developed and shipped highly interactive web applications for Apple Music using Ember.js</li>
                <li>Built and shipped the Apple Music Extension within Facebook Messenger leveraging third-party and internal APIs</li>
                <li>Architected and implemented the front-end of Apple Music\'s embeddable web player widget, which lets users log in and listen to full songs in the browser</li>
                <li>Contributed extensively to MusicKit.js, a JavaScript framework that allows developers to add an Apple Music player to their web apps</li>
            </ul>
        </div>
    </div>
</template>

<script>
    export default {
    }
</script>

<style scoped>
     h1 {
        font-size: 1.5rem;
        font-weight: 400;
        line-height: 1.2;
        margin-top: 0;
    }
    p {
        font-size: 1.3rem;
        margin-bottom: 1rem;
    }
    span {
         
         color: #69F7C1;
    }
    ul {
        list-style: inside linear-gradient( to right,#69F7C1,#69F7C1);
         border: 2px dashed transparent;
    }
    li {
        margin-bottom: 1rem;
        font-size: 1.3rem;
    }
    
     ul:hover {
         border: 2px dashed #69F7C1;
         padding: 2rem;
         margin: -2rem;
         margin-top: 0;
         box-sizing: border-box;
    }
</style>