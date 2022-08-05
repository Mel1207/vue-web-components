<template>
    <NavTopMini message="Version 1.0 Beta Test ⚡"/>
    <div class="navbar">
        <div class="nav-logo">
            <img src="../../assets/images/logo-main.svg" alt="">
        </div>
        
        <ul class="nav-menu">
            <NavLinks v-for="navLink in navLinks" :key="navLink.id" :title="navLink.item" :link="navLink.link"/>
            <li @click="openNav">
                <div class="hamburger-menu">
                    <div></div>
                    <div></div>
                </div>
            </li>
        </ul>
    </div>
    <NavbarMobile v-if="isOpen" @close="navClose"/>
</template>

<script>
import NavTopMini from './NavTopMini.vue'
import NavLinks from './NavLinks.vue'
import NavbarMobile from './NavbarMobile.vue'
import { ref } from '@vue/reactivity'

export default {
    components: {
        NavLinks,
        NavbarMobile,
        NavTopMini
    }, 
    setup() {
        const isOpen = ref(false)
        const navLinks = [
            {
                id: 1,
                item: 'Home',
                link: '/'
            },
            {
                id: 2,
                item: 'About',
                link: 'about'
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
            }
        ]

        const openNav = () => {
            isOpen.value = !isOpen.value
            console.log('nav is open')
        }

        const navClose = () => {
            isOpen.value = false
        }

        return {
            navLinks,
            isOpen,
            openNav,
            navClose
        }
    }
}
</script>