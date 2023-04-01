<template>
    <div class="card">
        <h3>{{ title }}</h3>
        <p>{{ description }}</p>
    </div>
</template>

<script>
export default {
    props: ['title', 'description']

}
</script>