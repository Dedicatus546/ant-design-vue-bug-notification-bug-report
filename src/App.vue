<script setup lang="ts">
import { ConfigProvider, notification } from "ant-design-vue";
import { onMounted } from "vue";

const [api, ContextHolder] = notification.useNotification({
  top: "80px",
});

onMounted(() => {
  api.info({
    message: "test",
    description: "test",
    duration: 0,
  });
});
</script>

<template>
  <ConfigProvider>
    App
    <context-holder />
  </ConfigProvider>
</template>

<style scoped></style>
