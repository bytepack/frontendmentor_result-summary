<script setup>
defineProps({
  title: {
    type: String,
    default: "Title"
  },
  score: {
    type: String,
    default: "50"
  },
  background: {
    type: String,
    default: "bg-yellow-700/50"
  },
  color: {
    type: String,
    default: "text-yellow-700"
  },
  icon: {
    type: String,
    required: "true"
  }
})
</script>
<template>
  <div
    :class="[background]"
    class="font-base font-bold flex justify-between rounded-2xl p-4"
  >
    <img class="w-5" :src="icon" :alt="title" />
    <h3 class="mr-auto ml-4" :class="[color]">{{ title }}</h3>
    <p class="text-slate-700/50">
      <span class="text-slate-700">{{ score }}</span> / 100
    </p>
  </div>
</template>
