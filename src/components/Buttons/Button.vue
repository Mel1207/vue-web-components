<template>
    <div class="btn" :class="type">
        {{ title }}
    </div>
</template>

<script>
export default {
    props: ['title', 'size', 'type']
}
</script>

<style>

</style>