<script setup>
import CardItem from "./components/CardItem.vue"
import IconReaction from "@/assets/images/icon-reaction.svg"
import IconMemory from "@/assets/images/icon-memory.svg"
import IconVerbal from "@/assets/images/icon-verbal.svg"
import IconVisual from "@/assets/images/icon-visual.svg"
</script>

<template>
  <main>
    <div
      class="font-hanken text-lg font-medium shadow-2xl sm:grid sm:grid-cols-2 sm:max-w-3xl sm:mx-auto sm:rounded-[2.2rem] sm:overflow-hidden"
    >
      <div
        class="flex flex-col gap-4 items-center justify-center bg-linear-225 from-violet-500 to-indigo-700 text-center px-10 pb-10 pt-5 rounded-b-[2.2rem] sm:rounded-b-none sm:gap-8"
      >
        <h3 class="text-indigo-200/80 text-xl font-bold">Your Result</h3>
        <div
          class="bg-linear-45 from-indigo-200/0 to-violet-800 w-[9rem] h-[9rem] rounded-full mx-auto flex items-center justify-center"
        >
          <h3 class="text-violet-200 text-lg">
            <span class="block font-extrabold text-6xl">76</span>of 100
          </h3>
        </div>

        <h3 class="text-indigo-50 font-bold text-2xl">Great</h3>
        <p class="text-indigo-100">
          You scored higher than 65% of the people who have taken these tests.
        </p>
      </div>

      <div class="p-7 bg-white">
        <h3 class="font-extrabold text-xl mb-5 text-slate-700">Summary</h3>
        <div class="card__items space-y-5">
          <CardItem
            title="Reaction"
            score="80"
            background="bg-rose-500/15"
            color="text-rose-500"
            :icon="IconReaction"
          />
          <CardItem
            title="Memory"
            score="92"
            background="bg-amber-400/15"
            color="text-amber-400"
            :icon="IconMemory"
          />
          <CardItem
            title="Verbal"
            score="61"
            background="bg-emerald-500/15"
            color="text-emerald-500"
            :icon="IconVerbal"
          />
          <CardItem
            title="Visual"
            score="72"
            background="bg-blue-700/15"
            color="text-blue-700"
            :icon="IconVisual"
          />
        </div>
        <a
          class="bg-slate-700 text-indigo-50 block text-center p-4 rounded-full font-bold text-base mt-5 transition-colors duration-300 hover:bg-indigo-700"
          href="#"
          >Continue</a
        >
      </div>
    </div>
  </main>
</template>
