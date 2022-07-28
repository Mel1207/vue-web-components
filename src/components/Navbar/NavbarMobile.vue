<template>
    <div class="navbar-mobile-menu">
        <button @click="closeNav">
            <img src="../../assets/images/icon-close.svg" alt="close">
        </button>

        <ul>
            <li v-for="link in navLinks" :key="link.id">{{ link.item }}</li>
        </ul>
    </div>
</template>

<script>
export default {
    emits: ['close'],
    setup(_, context) {
        const closeNav = () => {
            context.emit('close')
        }

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

        return {
            closeNav,
            navLinks
        }
    }
}
</script>