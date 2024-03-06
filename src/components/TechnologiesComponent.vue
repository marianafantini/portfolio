<script setup>
import {Image} from "ant-design-vue";

const languages = ["clojure", "cljs", "vuejs", "js", "elixir", "aws", "github", "postgresql"];
</script>

<template>
  <div class="image-list">
    <component
      v-for="language in languages"
      :key="language"
      :is="Image"
      :preview="false"
      class="image"
      height="3rem"
      :src="'./assets/' + language + '.svg'"
      :alt="language"
      :title="language"
    />
  </div>
</template>

<style>
.image {
  margin: 0.2rem;
}
@media (max-width: 1024px) {
  .image-list {
    padding: 1rem;
  }
}
</style>
