<template>
  <div class="button" :style="{ backgroundColor: bgcolor}">
    <p>{{ text }}</p>
  </div>
</template>

<script lang="ts" setup>
import { defineProps } from 'vue';

defineProps<{

  text: string
  bgcolor: string

}>()

</script>

<style scoped>

.button{
  color: white;
  border-radius: 5px;
  height: 30px;
  width: 130px;
  display: flex;
  justify-content: center;
  align-items: center;
  font-family: 'Quicksand', sans-serif;
  font-style: bold;
  box-shadow: rgba(51, 51, 51, 0.2) 0px 4px 16px 0px;
  transition: all 0.3s ease;
}

.button:hover {
  transform: translateY(-5px);
  box-shadow: rgba(51, 51, 51, 0.3) 0px 8px 24px 0px;
}

.button p {
  margin: 0;
  padding: 0;
}

</style>
