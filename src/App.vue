<template>
    <div>
        <app-header id="desktop"></app-header>
        <app-banner class="i"></app-banner>
        <app-social  class="i"></app-social>
        <app-about  class="i"></app-about>
        <app-experience  class="i"></app-experience>
        <app-project></app-project>
        <app-picture></app-picture>
        <app-contact></app-contact>
        <app-footer></app-footer>
       
    </div>
</template>

<script>
    import Header from './component/Header.vue'
    import Banner from './component/Banner.vue'
    import Social from './component/Social.vue'
    import About from './component/About.vue'
    import Experience from './component/Experience.vue'
    import Project from './component/Project.vue'
    import Contact from './component/Contact.vue'
    import Footer from './component/Footer.vue'
    import Picture from './component/Picture.vue'
   
    export default {
       components: {
           appHeader: Header,
           appBanner: Banner,
           appSocial: Social,
           appAbout: About,
           appExperience: Experience,
           appProject: Project,
           appPicture: Picture,
           appContact: Contact,
           appFooter: Footer
           
       }
    }
</script>

<style scoped>
body {
    position: relative;
}

/* .picture {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
}
.picture app-picture {
    margin-top: -100px;
} */

</style>