import type { NuxtLink } from '#build/components';
<template>
  <div class="send-form-section">
    <h2>Send your data</h2>
    <NuxtLink to="/feedback"
      ><button class="go-to-form">Go to form</button></NuxtLink
    >
  </div>
</template>

<script setup></script>

<style scoped>
.send-form-section {
  height: 262px;
  background-image: url(~/assets/svg/waves-background.svg);
  padding: 105px;
  display: flex;
  justify-content: space-between;
}
h2 {
  color: #fff;
}
button {
  width: 392px;
  border: none;
  border-radius: 100px;
  background-color: var(--color-accent);
  display: flex;
  height: 58px;
  padding: 10px 24px;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  gap: 10px;
  flex-shrink: 0;
  color: #fff;
  font-size: 18px;
  line-height: 28px;
}
</style>
