<script setup>
import {Typography} from "ant-design-vue";
const {Title} = Typography;
import QualificationCardComponent from "@/components/QualificationCardComponent.vue";

const qualifications = [
  {
    title: "Diverse Background",
    description:
      "I've worked with both frontend and backend technologies, allowing me to bridge the gap seamlessly",
  },
  {
    title: "Deep Technical Knowledge",
    description:
      "Over 6 years of industry experience, and counting. Experience with both internal and user-facing products",
  },
  {
    title: "User-Centric Approach",
    description: "My designs prioritize user needs, resulting in intuitive interfaces",
  },
  {
    title: "Collaborative Spirit",
    description: "I enjoy collaborating with cross-functional teams to create impactful solutions",
  },
];
</script>

<template>
  <div class="qualifications">
    <Title :level="3">Why me?</Title>

    <div class="qualification-list">
      <component
        v-for="qualification in qualifications"
        :key="qualification"
        :is="QualificationCardComponent"
        :title="qualification.title"
        :description="qualification.description"
      >
      </component>
    </div>
  </div>
</template>

<style>
.qualification-list {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(230px, 1fr));
  justify-content: space-evenly;
}
@media (max-width: 1024px) {
  .qualifications {
    padding: 1rem;
  }
}
</style>
