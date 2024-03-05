<script setup>
import {Avatar} from "ant-design-vue";

const languages = ["clojure", "cljs", "vuejs", "js", "elixir", "aws", "github", "postgresql"];
</script>

<template>
  <div class="avatar-list">
    <component
      v-for="language in languages"
      :key="language"
      :is="Avatar"
      class="avatar"
      shape="square"
      size="large"
      :src="'/portfolio/assets/' + language + '.svg'"
      :alt="language"
      :title="language"
    />
  </div>
</template>

<style>
.avatar {
  margin: 0.2rem;
}
@media (max-width: 1024px) {
  .avatar-list {
    padding: 1rem;
  }
}
</style>
