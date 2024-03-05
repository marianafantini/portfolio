<script setup>
import {Typography, Avatar} from "ant-design-vue";
const {Title} = Typography;
import PresentationComponent from "../components/PresentationComponent.vue";
import AboutComponent from "../components/AboutComponent.vue";
import ContactComponent from "../components/ContactComponent.vue";
import PortfolioComponent from "../components/PortfolioComponent.vue";
import QualificationsComponent from "../components/QualificationsComponent.vue";
import TechnologiesComponent from "../components/TechnologiesComponent.vue";
</script>

<template>
  <div class="presentation-section">
    <PresentationComponent></PresentationComponent>
  </div>

  <div class="content-section">
    <AboutComponent></AboutComponent>
    <TechnologiesComponent></TechnologiesComponent>
    <PortfolioComponent></PortfolioComponent>
    <QualificationsComponent></QualificationsComponent>
    <ContactComponent></ContactComponent>
  </div>
</template>

<style scoped>
@media (min-width: 1024px) {
  .presentation-section {
    width: 30vw;
  }
  .content-section {
    width: 70vw;
  }
}
</style>
