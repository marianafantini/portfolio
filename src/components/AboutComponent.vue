<script setup>
import {Typography} from "ant-design-vue";
const {Title, Paragraph} = Typography;
import TechnologiesComponent from "@/components/TechnologiesComponent.vue";

</script>

<template>
  <div class="about">
    <Title :level="3">< / About ></Title>
    <Paragraph class="about-paragraph">
      As a full-stack developer with over 6 years of industry experience, I enjoy solving complex
      problems and crafting direct, user-friendly interfaces. My journey has led me through diverse
      projects, from backend architecture to pixel-perfect frontend design.
    </Paragraph>
    <TechnologiesComponent></TechnologiesComponent>
  </div>
</template>

<style>
.about-paragraph {
  font-size: 1rem;
}
@media (max-width: 1024px) {
  .about {
    padding: 1rem;
  }
}
</style>
