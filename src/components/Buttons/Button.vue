<template>
    <div class="btn" :class="type">
        {{ title }}

        <!-- <img :src="require(`../../assets/images/${minIcon}`)" alt="github"> -->
    </div>
</template>

<script>
export default {
    props: ['title', 'size', 'type', 'minIcon']
}
</script>

<style>

</style>