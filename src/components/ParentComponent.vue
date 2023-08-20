<script setup>
import {ref} from "vue";
import ChildComponent from "@/components/ChildComponent.vue";
const msg = ref('Hi I am a Vue Learner!')
</script>

<template>
<section class="mx-auto container my-10">
  <h2 class="text-3xl font-bold text-green-500 my-5 text-center border-y-2 py-3 border-green-300">Parent Component</h2>
  <p class="text-lg font-semibold text-center text-gray-500" >{{ msg }}</p>
  <ChildComponent v-model="msg"/>
</section>
</template>

<style scoped>

</style>