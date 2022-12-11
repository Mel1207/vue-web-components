<template>
    <div class="container">
        <div class="flex item-center">
            <h2>Text about</h2>
            <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Molestiae voluptates nostrum tempora!</p>
            <Button title="Learn More" type="btn-primary" />
            <br>
            <Card v-for="cardItem in cardItems" :key="cardItem.id"/>
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
        const cardItems = [
            { 
                title: 'title 1',
                description: 'lorem ipsum dolor sit amet'
            },
            { 
                title: 'title 2',
                description: 'lorem ipsum dolor sit amet'
            },
            { 
                title: 'title 3',
                description: 'lorem ipsum dolor sit amet'
            },
            { 
                title: 'title 4',
                description: 'lorem ipsum dolor sit amet'
            }
        ]



        return {
            cardItems
        }
    }

}
</script>

<style>

</style>