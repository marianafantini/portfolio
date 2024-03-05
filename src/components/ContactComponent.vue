<script setup>
import {Typography} from "ant-design-vue";
const {Title, Paragraph} = Typography;
</script>

<template>
  <div class="contact">
    <Title :level="3">Get in touch!</Title>
 
    <Paragraph>Feel free to email me at mariana.fantini.dev@gmail.com</Paragraph>
  </div>
</template>

<style>
@media (max-width: 1024px) {
  .contact {
    padding: 1rem;
  }
}
</style>
