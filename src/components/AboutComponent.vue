<script setup>
import {Typography} from "ant-design-vue";
const {Title, Paragraph} = Typography;
</script>

<template>
  <div class="about">
    <Title :level="3">< / About ></Title>
    <Paragraph>
      As a full-stack developer with over 6 years of industry experience, I enjoy solving complex
      problems and crafting direct, user-friendly interfaces. My journey has led me through diverse
      projects, from backend architecture to pixel-perfect frontend design.
    </Paragraph>
  </div>
</template>

<style>
@media (max-width: 1024px) {
  .about {
    padding: 1rem;
  }
}
</style>
