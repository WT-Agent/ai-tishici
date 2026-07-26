<template>
  <div class="glass-card ticker-card">
    <div class="ticker-wrapper">
      <div v-for="(item, index) in tickerItems" :key="index" class="ticker-item">
        <span>{{ item.text }}</span>
        <span style="color: var(--success-color); font-weight: bold;">[生成完成]</span>
      </div>
    </div>
  </div>
</template>

<script setup lang="ts">
import { ref } from 'vue';

const tickerItems = ref([
  {
    "text": "用户 138****5500 将普通写周报指令升级为 CO-STAR 高效 Prompt"
  },
  {
    "text": "用户 189****9911 获得了 Midjourney 商业摄影高清 Prompt"
  },
  {
    "text": "用户 131****4422 完成了让 Claude 严格输出 JSON 结构的约束指令"
  },
  {
    "text": "用户 156****7788 生成了思维链 (CoT) 复杂逻辑推理 Prompt"
  },
  {
    "text": "用户 173****3311 取得了自制大模型 Agent 机器人系统提示词"
  }
]);
</script>
