<script setup>
import {Typography, Avatar} from "ant-design-vue";
const {Title} = Typography;
</script>

<template>
  <div class="presentation-section">
    <img
      alt="Profile photo"
      class="profile-photo"
      src="/portfolio/assets/foto-rosto-MarianaFantini.jpeg"
      width="250"
    />
    <Title :level="2">Mariana Fantini</Title>
    <Title :level="4" class="presentation-description">Software Engineer (she/her)</Title>
    <div>
      <a target="_blank" href="https://www.github.com/marianafantini/">
        <Avatar shape="square" src="/portfolio/assets/github.svg"></Avatar>
      </a>
      <a target="_blank" href="https://www.linkedin.com/in/marianafantini/">
        <Avatar shape="square" src="/portfolio/assets/linkedin.svg"></Avatar>
      </a>
    </div>
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
  padding: 1rem;
}
.presentation-description {
  margin-top: 0;
}
</style>
