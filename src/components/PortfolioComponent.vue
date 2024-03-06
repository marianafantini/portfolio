<script setup>
import {Typography, Image} from "ant-design-vue";
const {Title, Paragraph} = Typography;
const githubUrl = "https://github.com/marianafantini/";
const previousWork = [
  {
    title: "dog-ngo-canva-website",
    tech: "vuejs",
    website: "https://marianafantini.github.io/dog-ngo-canva-website/"
  },
  {
    title: "portfolio",
    tech: "vuejs",
  },
  {
    title: "angular-tour-of-heroes",
    tech: "angular",
  },
  {
    title: "tic-tac-toe-tutorial",
    tech: "react",
  },
];
</script>

<template>
  <div class="portfolio">
    <Title :level="3">Previous work</Title>
    <Paragraph>My github repositories:</Paragraph>
    <ul v-for="work in previousWork" :key="work.title">
      <Image
        height="1rem"
        :preview="false"
        shape="square"
        :src="'./assets/' + work.tech + '.svg'"
      ></Image>
      <a target="_blank" :href="githubUrl + work.title">
        {{ work.title }} code
      </a>
      <span v-if="work.website"> - 
      <a target="_blank" :href="work.website">
        preview website
      </a>
      </span>
    </ul>
  </div>
</template>

<style>
@media (max-width: 1024px) {
  .portfolio {
    padding: 1rem;
  }
}
</style>
