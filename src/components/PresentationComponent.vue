<script setup>
import {Typography, Avatar} from "ant-design-vue";
const {Title} = Typography;
</script>

<template>
  <div class="presentation-section">
    <img
      alt="Profile photo"
      class="profile-photo"
      src="/assets/foto-rosto-MarianaFantini.jpeg"
      width="250"
    />
    <Title class="presentation-name" :level="2">Mariana Fantini</Title>
    <Title class="presentation-description" :level="4">Software Engineer (she/her)</Title>
  </div>
</template>

<style scoped>
.presentation-section {
  display: flex;
  flex-direction: column;
  align-items: center;
  padding: 2rem;
}
.presentation-section .profile-photo {
  padding: 0rem 1rem;
}
.presentation-name {
  margin-bottom: 0;
}
.presentation-description {
  margin-top: 0 !important;
}
</style>
