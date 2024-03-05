<script setup>
import {Card} from "ant-design-vue";
const props = defineProps(['title', 'description'])
</script>

<template>
  <Card class="qualification-card" size="small">
    <h3 v-if="props?.title">{{ props.title }}</h3>
    <p v-if="props?.description">{{ props.description }}</p>
  </Card>
</template>

<style>
.qualification-card {
  margin: 0.5rem;
}
</style>
