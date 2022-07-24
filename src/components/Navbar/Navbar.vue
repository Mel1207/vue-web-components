<template>
    <div class="navbar">
        <div class="nav-logo">
            <img src="../../assets/images/logo-main.svg" alt="">
        </div>
        

        <ul class="nav-menu">
            <li><a href="#!">Home</a></li>
            <li><a href="#!">About</a></li>
            <li><a href="#!">Blogs</a></li>
            <li><a href="#!">Contacts</a></li>
        </ul>
    </div>
</template>

<script>
export default {
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