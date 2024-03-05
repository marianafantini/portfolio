<script setup>
import QualificationCardComponent from "../components/QualificationCardComponent.vue";

const qualifications = [
  {
    title: "Technical Depth",
    description:
      "I've worked with both frontend and backend technologies, allowing me to bridge the gap seamlessly",
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
</template>

<style>
.qualification-list {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
  justify-content: space-evenly;
}
@media (max-width: 1024px) {
  .qualification-list {
    padding: 1rem;
  }
}
</style>
