<template>
    <div class="navbar-mobile-menu">
        <button @click="closeNav">Close me</button>
    </div>
</template>

<script>
export default {
    emits: ['close'],
    setup(_, context) {
        const closeNav = () => {
            context.emit('close')
        }

        return {
            closeNav
        }
    }
}
</script>