<script setup>
import {Typography, Avatar} from "ant-design-vue";
const {Title} = Typography;
</script>

<template>
  <div class="contact">
    <Title :level="5">Contact me</Title>
    <div>
      <a target="_blank" href="mailto:mariana.fantini.dev@gmail.com">
        <Avatar shape="square" src="./assets/email.svg"></Avatar>
      </a>
      <a target="_blank" href="https://www.github.com/marianafantini/">
        <Avatar shape="square" src="./assets/github.svg"></Avatar>
      </a>
      <a target="_blank" href="https://www.linkedin.com/in/marianafantini/">
        <Avatar shape="square" src="./assets/linkedin.svg"></Avatar>
      </a>
    </div>
  </div>
</template>

<style>
a {
  padding: 0.2rem;
}
</style>
