<template>
    <div class="container">
        <div class="flex item-center">
            <h2>Text about</h2>
            <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Molestiae voluptates nostrum tempora!</p>
            <Button title="Learn More" type="btn-primary" />
        </div>
        <img src="" alt="">
    </div>
</template>

<script>
import Button from '../Buttons/Button.vue' 

export default {
    props: ['title', 'type'],
    components: { Button },
    setup() {
    }

}
</script>

<style>

</style>