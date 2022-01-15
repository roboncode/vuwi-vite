<script setup lang="ts">
// This starter template is using Vue 3 <script setup> SFCs
// Check out https://v3.vuejs.org/api/sfc-script-setup.html#sfc-script-setup
import { ref } from 'vue-demi';
import HelloWorld from './components/HelloWorld.vue'
import VButton from './modules/vuwi/components/Button/VButton.vue';
import VTextInput from './modules/vuwi/components/TextInput/VTextInput.vue';
import VLine from './modules/vuwi/components/Line/VLine.vue';
import VSpinner from './modules/vuwi/components/Spinner/VSpinner.vue';

const text = ref('')
</script>

<template>
  <img alt="Vue logo" src="./assets/logo.png" />
  <HelloWorld msg="Hello Vue 3 + TypeScript + Vite" />
  <div class="flex flex-col w-full items-center">
    <div class="w-full max-w-lg p-4 space-y-2">
      <VTextInput label="Name" v-model="text" class="border wi-border" />
      <VButton size="xl" class="wi-primary w-full">Submit</VButton>
    </div>
  </div>
</template>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
