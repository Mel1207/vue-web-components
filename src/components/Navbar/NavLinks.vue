<template>
    <router-link :to="link"><li>{{ title }}</li></router-link>
</template>

<script>
export default {
    props: [ 'title', 'link' ]
}
</script>