<template>
    <div class="header container">
        <div>
            <h1>Designed to Build Your <br> Component 
                <span class="header-highlight">Lightning Fast</span>
            </h1>
            <p>
                Lorem Ipsum is simply dummy text of the printing and typesetting <br> industry.'s standard dummy text ever since the 1500s
            </p>

            <div class="controls">
                <Button title="Get Started" type="btn-primary"/>
                <Button title="Documentation" type="btn-secondary"/>
            </div>
        </div>
    </div>
</template>

<script>
import Button from '../Buttons/Button.vue'

export default {
    components: { Button }
}
</script>