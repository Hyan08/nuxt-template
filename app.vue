<template>
  <n-config-provider :theme="theme">
    <n-global-style />
    <NuxtLayout>
      <NuxtLoadingIndicator />
      <NuxtPage></NuxtPage>
    </NuxtLayout>
  </n-config-provider>
</template>
<script setup lang="ts">
import { NConfigProvider, NGlobalStyle } from 'naive-ui'
import type { GlobalTheme } from 'naive-ui'
// 全局的主题
const theme = ref<GlobalTheme | null>(null)
</script>
