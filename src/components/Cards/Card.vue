<template>
  <div class="card">
    <h2 class="h4">{{ title }}</h2>
    <p>{{ description }}</p>
  </div>
</template>

<script>
export default {
  props: ["title", "description"],
};
</script>
