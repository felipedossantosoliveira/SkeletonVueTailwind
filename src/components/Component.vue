<script>
export default {
  name: "Component",
  data() {
    return {
      repeats: 6,
    };
  },
};
</script>
<template>
  <div class="w-full h-96 bg-slate-900">
    <h1 class="text-lg text-neutral-100 font-bold p-4">Para DarkMode</h1>
    <div class="p-4 grid grid-cols-3 gap-2">
      <div
        v-for="(reapeat, index) in repeats"
        :key="index"
        class="bg-slate-800 px-4 py-3 rounded-md animate-pulse space-x-3 flex"
      >
        <div>
          <div class="w-8 h-8 rounded-full bg-slate-700"></div>
        </div>
        <div class="grid gap-y-2 w-full">
          <div class="w-2/3 h-2 mb-2 rounded-full bg-slate-700"></div>
          <div class="w-full h-1 rounded-full bg-slate-700"></div>
          <div class="w-full h-2 rounded-full bg-slate-700"></div>
          <div class="w-full h-1 rounded-full bg-slate-700"></div>
        </div>
      </div>
    </div>
  </div>
  <div class="w-full h-96 bg-slate-50">
    <h1 class="text-lg font-bold p-4">Para LightMode</h1>
    <div class="p-4 grid grid-cols-3 gap-2">
      <div
        v-for="(reapeat, index) in repeats"
        :key="index"
        class="bg-slate-200 px-4 py-3 rounded-md animate-pulse space-x-3 flex"
      >
        <div>
          <div class="w-8 h-8 rounded-full bg-slate-300"></div>
        </div>
        <div class="grid gap-y-2 w-full">
          <div class="w-2/3 h-2 mb-2 rounded-full bg-slate-300"></div>
          <div class="w-full h-1 rounded-full bg-slate-300"></div>
          <div class="w-full h-2 rounded-full bg-slate-300"></div>
          <div class="w-full h-1 rounded-full bg-slate-300"></div>
        </div>
      </div>
    </div>
  </div>
</template>

