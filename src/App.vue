<script setup>
import {Layout, ConfigProvider} from "ant-design-vue";
import ContentView from "./views/ContentView.vue";
const {Header, Content} = Layout;

</script>

<template>
    <ConfigProvider
    :theme="{
      // token: { fontSize: 18}
    }"
  >
  <Layout class="layout">
    <Header class="header"></Header>

    <Layout>
      <Content class="content">
        <ContentView></ContentView>
      </Content>
    </Layout>
  </Layout>
</ConfigProvider>
</template>

<style scoped>
.layout {
  height: 100vh;
}
.header {
  display: flex;
  position: sticky;
}

@media (min-width: 1024px) {
  .content {
    display: flex;
    padding: 2rem;
  }
  .presentation-section {
    width: 30vw;
    display: flex;
    flex-direction: column;
    align-items: center;
    padding: 2rem;
    position: sticky;
  }
  .presentation-section .profile-photo {
    padding: 1rem;
  }
  .content-section {
    width: 70vw;
  }
}
</style>
