<template>
    <div>
        <div class="navbar">
            <div class="navbar__toggle">
                <span></span>
            </div>
            <div class="navbar__logo">
                <a href="">Navbar Logo</a>
            </div>
            <nav class="navbar__nav">
                <ul class="navbar__menu">
                    <li class="navbar__list">
                        <a href="" class="navbar__link"><span>01.</span> About</a>
                    </li>
                    <li class="navbar__list">
                        <a href="" class="navbar__link"><span>02.</span> Experience</a>
                    </li>
                    <li class="navbar__list">
                        <a href="" class="navbar__link"><span>03.</span> Work</a>
                    </li>
                    <li class="navbar__list">
                        <a href="" class="navbar__link"><span>04.</span> Contact</a>
                    </li>
                </ul>
                <button class="btn nav-btn">Resume</button>
            </nav>
        </div>
    </div>
</template>

<script>

    export default {
       
    }
</script>

<style scoped>
    .navbar {
        height: 6rem;
        display: flex;
        justify-content: space-between;
        align-items: center;
        background-color: rgba(0, 0, 0, 0.99);
        padding: 5rem 9rem;
    }

    .navbar__nav {
        display: flex;
        align-items: center;
        justify-content: center;
    }
    .navbar__menu {
        display: flex;
        align-items: center;
        justify-content: center;
        list-style: none;
    }

    .navbar__list {
         margin-right: 3rem;
    }

    .navbar__link {
        display: inline-block;
        text-decoration: none;
        color: #eee;
        padding: 1rem;
        font-size: 1.4rem;
        transition: color 1s;
    }

    .navbar__link:hover {
        color: #69f7c1;
    }

    .navbar__link span {
        color: #69f7c1;
        margin-right: .3rem;
    }
    .navbar__logo a {
        position: fixed;
        top: 3rem;
        left: 3rem;
        font-weight: bold;
        font-size: 2rem;
        color: white;
        text-decoration: none;
    }

    @media screen and (max-width: 56.25em) {
        .navbar {
            position: fixed;
            top: 0;
            right: 0;
            padding: 0;
            width: 60%;
            height: 100vh;
            justify-content: center;
            align-items: center;
            flex-direction: column;
            background: black;
            display: none;
        }

        .navbar__nav {
            flex-direction: column;
        }

        .navbar__menu {
            flex-direction: column;
        }

         .navbar__list {
         margin-right: 0;
         margin: 1rem auto;
         }

         .navbar__link {
        display: inline-block;
        text-decoration: none;
        color: #eee;
        padding: 1rem;
        font-size: 3rem;
    }

    .nav-btn {
        margin-top: 3rem;
        font-size: 1.5rem;
    }
    .navbar__toggle {
        position: fixed;
        top: 4rem;
        right: 6rem;
         
        z-index: 20000;
    }
    .navbar__toggle span {
        display: inline-block;
        width: 2.5rem;
        height: .2rem;
        background-color: #eee;
        position: relative;
       
    }

    .navbar__toggle span::after,
    .navbar__toggle span::before {
        display: inline-block;
        content: '';
        position: absolute;
        right: 0;
        height: .2rem;
        background-color: #eee;
    }


     .navbar__toggle span::after {
         top: 1rem;
         width: 2rem;
     }
     .navbar__toggle span::before {
         top: -1rem;
         width: 3rem;
     }


}
    
</style>