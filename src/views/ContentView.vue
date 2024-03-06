<script setup>
import {Divider} from "ant-design-vue";
import PresentationComponent from "@/components/PresentationComponent.vue";
import AboutComponent from "@/components/AboutComponent.vue";
import ContactComponent from "@/components/ContactComponent.vue";
import QualificationsComponent from "@/components/QualificationsComponent.vue";
import PortfolioComponent from "@/components/PortfolioComponent.vue";
</script>

<template>
  <div class="presentation-section">
    <Space class="presentation-space">
      <PresentationComponent></PresentationComponent>
      <ContactComponent></ContactComponent>
    </Space>
  </div>

  <div class="content-section">
    <Space class="content-space" :direction="horizontal">
      <AboutComponent class="about"></AboutComponent>
      <PortfolioComponent class="portfolio"></PortfolioComponent>
    </Space>
    <Divider></Divider>
    <QualificationsComponent></QualificationsComponent>
  </div>
</template>

<style scoped>
@media (max-width: 1024px) {
  .presentation-space {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
  }
  .presentation-space .presentation-section {
    padding-bottom: 0;
  }
  .presentation-space .contact {
    display: flex;
    flex-direction: column;
    align-items: center;
  }
}
@media (min-width: 1024px) {
  .about {
    max-width: 50%;
  }
  .portfolio {
    max-width: 50%;
  }
  .content-space {
    display: flex;
  }
  .presentation-space {
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    height: 100%;
  }
  .presentation-section {
    width: 30vw;
  }
  .content-section {
    width: 70vw;
  }
}
</style>
