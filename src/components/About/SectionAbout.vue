<template>
    <div class="container">
        <div class="flex item-center">
            <h2>Text about</h2>
            <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Molestiae voluptates nostrum tempora!</p>
            <Button title="Learn More" type="btn-primary" />
            <br>
            <Card />
        </div>
        <img src="" alt="">
        <!-- to add image -->
    </div>
</template>

<script>
import Button from '../Buttons/Button.vue' 
import Card from '../Cards/Card.vue'

export default {
    props: ['title', 'type'],
    components: { Button, Card },
    setup() {
    }

}
</script>

<style>

</style>