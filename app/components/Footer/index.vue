<!--
 * @Author: 白雾茫茫丶<baiwumm.com>
 * @Date: 2024-05-30 13:52:19
 * @LastEditors: 白雾茫茫丶<baiwumm.com>
 * @LastEditTime: 2025-07-30 08:59:22
 * @Description: 底部布局
-->
<template>
  <footer class="px-4 py-2">
    <USeparator
      :avatar="{
        src: '/logo.svg',
      }"
    />
    <div class="flex justify-between items-center max-sm:flex-col">
      <!-- 社交图标 -->
      <div class="max-sm:order-first">
        <!-- 社交图标 -->
        <SocialIcon
          v-for="({ icon, url, tip }, index) in FooterSocial"
          :key="index"
          :icon="icon"
          :url="url"
          :tip="tip"
        />
      </div>
    </div>
  </footer>
</template>
<script setup lang="ts">
import { FooterSocial, FooterRecord } from "~/lib/constant";
</script>
