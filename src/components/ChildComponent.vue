<script setup>
defineProps(['modelValue'])
function getCustomMessage(){
  return 'Custom Message from Child Component!'
}
</script>

<template>
<section class="my-16">
  <h2 class="text-3xl font-bold text-red-500 my-5 text-center border-y-2 py-3 border-red-300">Child Component</h2>
  <p class="text-lg font-semibold text-center text-gray-500" >{{ modelValue }}</p>
  <div class="flex items-center justify-center my-5">
    <button class="bg-red-500 px-6 py-2 rounded text-white text-center" @click="$emit('update:modelValue', getCustomMessage())">Custom Message</button>
  </div>

</section>
</template>

<style scoped>

</style>