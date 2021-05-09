<template>
    <section class="experience">
        <div class="container">
            <div class="text-line mb">
                <h3 class="heading-3"><span>02.</span>Where i've worked</h3>
            </div>
            <div class="tab">
                <div class="tab-right">
                    <ul class="nav-menu">
                        <li class="nav-list"><span>Upstatement</span></li>
                        <li class="nav-list" @click="one">Apple</li>
                        <li class="nav-list" @click="two">Scout</li>
                        <li class="nav-list" @click="three">Mullenlowe</li>
                    </ul>
                </div>
                <div class="tab-left">
                    <component :is="selectedTab"></component>
                </div>
            </div>
    </div>
    </section>
</template>

<script>
import Tab3  from './Tabs/Tab3.vue'
import Tab2  from './Tabs/Tab2.vue'
import Tab1  from './Tabs/Tab1.vue'
    export default {
        data() {
            return {
                selectedTab: 'tabThree'
            }
        },
        components: {
            tabThree: Tab3,
            tabTwo: Tab2,
            tabOne: Tab1
        },
        methods: {
            one() {
               this.selectedTab = 'tabOne';
            },
            two() {
                this.selectedTab = 'tabTwo';
            },
            three() {
                 this.selectedTab = 'tabThree';
            }
        }
    }
</script>

<style scoped>


.mb {
    margin-bottom: 6rem;
}

.experience {
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

    .tab {
        display: flex;
        justify-content: center;
    }

    .tab-right {
        flex: 50%;
    }
    .tab-left {
        flex: 50%;
        margin-left: -1 0rem;
    }






    .nav-menu {
        list-style: none;
        width: 50%;
        margin-left: auto;
    }
    .nav-list {
        font-size: 1.5rem;
        padding: 1rem 2rem;
        border-left: 2px solid #aaa;
        cursor: pointer;
        transition: all .5s;
    }
    .nav-list:hover {
        background-color: #011;
        border-color: #69F7C1;
    }

    @media screen and (max-width: 68.75em) {
        .tab {
            flex-direction: column;
        }
        .nav-menu {
            list-style: none;
            width: 70%;
            margin: 0 auto;
            text-align: center;
            /* margin-left: 0; */
        }
        .nav-list {
            display: inline-block;
            border-left: none;
            border-bottom: 2px solid #aaa;
            margin-right: 1rem;
        }

        .tab-right {
            margin-bottom: 5rem;
        }
        .tab-left {
            /* text-align: center; */
        }
    }

</style>