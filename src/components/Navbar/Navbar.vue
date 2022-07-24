<template>
    <div class="navbar">
        <div class="nav-logo">
            <img src="../../assets/images/logo-main.svg" alt="">
        </div>
        
        <ul class="nav-menu">
            <NavLinks v-for="navLink in navLinks" :key="navLink.id" :title="navLink.item" :link="navLink.link"/>
        </ul>
    </div>
    
</template>

<script>
import NavLinks from './NavLinks.vue'

export default {
    components: {
        NavLinks
    }, 
    setup() {
        const navLinks = [
        {
            id: 1,
            item: 'Home',
            link: '/'
        },
        {
            id: 2,
            item: 'About',
            link: '/About'
        },
        {
            id: 3,
            item: 'Blogs',
            link: '/Blogs'
        },
        {
            id: 4,
            item: 'Contacts',
            link: '/Contacts'
        },
    ]

        return {
            navLinks
        }
    }
}
</script>