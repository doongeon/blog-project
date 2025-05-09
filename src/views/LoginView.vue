<template>
  <div>
    <div class="max-w-md mx-auto mt-20 shadow-lg rounded-lg">
      <div class="px-10 py-5">
        <div class="text-center font-bold text-2xl py-7">로그인</div>
        <hr class="text-gray-300" />
        <div class="mt-5 px-1">
          <div>
            <label class="" for="id">아이디</label>
          </div>
          <div>
            <input
              disabled
              class="mt-3 py-px px-1 w-full border border-gray-300 rounded-md disabled:bg-gray-300"
              type="text"
              name="id"
              id="id"
              v-model="state.id"
              placeholder="ID"
            />
          </div>
        </div>
        <div class="mt-5">
          <div>
            <label for="password">패스워드</label>
          </div>
          <div>
            <input
              disabled
              class="mt-3 py-px px-1 w-full border border-gray-300 rounded-md disabled:bg-gray-300"
              type="password"
              name="password"
              id="password"
              v-model="state.password"
              placeholder="PW"
            />
          </div>
        </div>
        <hr class="text-gray-300 mt-5" />
        <div>
          <ul class="flex justify-center">
            <li>a</li>
            <li class="pl-5">b</li>
          </ul>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup lang="ts">
import { reactive } from 'vue';
const state = reactive({ id: '', password: '' });
</script>
