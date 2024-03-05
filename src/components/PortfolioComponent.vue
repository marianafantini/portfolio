<script setup>
import {Typography} from "ant-design-vue";
const {Title} = Typography;
</script>

<template>
  <div class="portfolio">
    <Title :level="3">Previous work</Title>
  </div>
</template>

<style>
@media (max-width: 1024px) {
  .portfolio {
    padding: 1rem;
  }
}
</style>
