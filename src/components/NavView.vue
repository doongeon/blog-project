<template>
  <nav id="nav" class="flex bg-green-800 py-5 px-5 text-green-50 justify-between text-base">
    <button @click="shootConfetti">
      <i class="fa-solid fa-palette text-lg"></i>
    </button>
    <div class="flex gap-5">
      <RouterLink :to="{ name: 'home' }">홈</RouterLink>
      <RouterLink :to="{ name: 'posts' }">포스트</RouterLink>
    </div>
    <RouterLink disabled :to="{ name: 'login' }">로그인</RouterLink>
  </nav>
</template>

<script setup lang="ts">
import confetti from 'canvas-confetti';
import { RouterLink } from 'vue-router';

const shootConfetti = () => {
  confetti({
    particleCount: 150,
    spread: 100,
    origin: { y: 0.6 },
  });
};
</script>
