<script setup lang="ts">

import {ref} from "vue";

const buttonStatus = ref(true)

const handleClick = () => {
  buttonStatus.value = !buttonStatus.value
  console.log('buttonStatus', buttonStatus.value)
}

</script>

<template>
  <div class="space-y-4">
    <div @click="handleClick" class="bg-white p-4 rounded-2xl text-center font-semibold text-blue-400">Click me</div>
    <div class="border border-white p-4 text-white font-semibold text-center rounded-2xl">
      {{ buttonStatus }}
    </div>
  </div>
</template>
