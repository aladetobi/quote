<template>
    <div>
       <div>
            <div class="div" v-for="(outer, index) in outerList" :key="index">
                <h3>{{ outer.head }}</h3>
                <span>{{ outer.span }}</span>
                <p>{{ outer.list[0] }}</p>
                <ul>
                    <li v:for="(l, index) in list" :key="index">{{ l }}</li>
                </ul>
            </div>
        </div>
    </div>
</template>
<script>
    export default {
        data() {
            return {
                    outerList: [
                        {
                            head:  'UI Frontrend Co-op @ Apple',
                            span: 'July - December 2017',
                            list: 
                                [
                                   'Lorem ipsum',
                                    'Built and shipped the Apple Music Extension within Facebook Messenger leveraging third-party and internal APIs',
                                   'Architected and implemented the front-end of Apple Music\'s embeddable web player widget, which lets users log in and listen to full songs in the browser',
                                   'Contributed extensively to MusicKit.js, a JavaScript framework that allows developers to add an Apple Music player to their web apps'
                                ]
                        },
                        {
                             head:  'UI Backend Co-op @ Apple',
                             span: 'July - December 2017',
                            list: 
                                {
                                    one: 'Lorem ipsum',
                                    two: 'Built and shipped the Apple Music Extension within Facebook Messenger leveraging third-party and internal APIs',
                                    three: 'Architected and implemented the front-end of Apple Music\'s embeddable web player widget, which lets users log in and listen to full songs in the browser',
                                    four: 'Contributed extensively to MusicKit.js, a JavaScript framework that allows developers to add an Apple Music player to their web apps'
                                }
                        },
                        {
                            head:  'UI Engineer Co-op @ Apple',
                            span: 'July - December 2017',
                            list: 
                                {
                                    one: 'Developed and shipped highly interactive web applications for Apple Music using Ember.js',
                                    two: 'Built and shipped the Apple Music Extension within Facebook Messenger leveraging third-party and internal APIs',
                                    three: 'Architected and implemented the front-end of Apple Music\'s embeddable web player widget, which lets users log in and listen to full songs in the browser',
                                    four: 'Contributed extensively to MusicKit.js, a JavaScript framework that allows developers to add an Apple Music player to their web apps'
                                    
                                }
                        }
                    ]
            }
        }
    }
</script>

<style scoped>
div {
    height: 100vh;
}
     h1 {
        font-size: 20px;
        line-height: 1.2;
         margin-bottom: 30px;
        margin-top: 0;
    }
    span {
        color: #69F7C1;
    }
    .nav {
        list-style: none;
        width: 20%;
    }
    .nav li {
        color: #000;
        padding: 10px 20px 10px 15px;
        border-left: 2px solid #aaa;
        cursor: pointer;
    }
    .nav li:hover {
        background-color: #444;
    }
    .nav li:hover {
        border-left-color: #69F7C1;
    }
    .second-list li {
        font-size: 14px;
        margin-bottom: 10px;
    }
    .bod {
        width: 600px;
        height: 100%;
        padding: 10px;
        margin-top: 50px;
    }
    .bod:hover {
         border: 2px dashed #69F7C1;
    }
    li {
        color: #000;
        font-size: 5rem;
        padding: 10px 20px 10px 15px;
        border-left: 2px solid #aaa;
        cursor: pointer;
    }
</style>