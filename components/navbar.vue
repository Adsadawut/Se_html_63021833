<template>
  <div
    class="h-auto bg-green-500 p-4 flex flex-wrap justify-center items-center"
  >
    <div class="w-1/3">
      <button @click="menu = !menu" class="ml-4">menu</button>
    </div>
    <div class="w-1/3">
      <center class="text-xl text-white">Homepage</center>
    </div>
    <div class="w-1/3 flex justify-end">
      <button class="mr-4">Profile</button>
    </div>
    <div v-if="menu" class="w-full flex flex-col">
      <button class="p-2 m-2 text-white hover:bg-green-400">Notebook</button>
      <button class="p-2 m-2 text-white hover:bg-green-400">Notebook Gaming</button>
      <button class="p-2 m-2 text-white hover:bg-green-400">Notebook 2in1</button>
    </div>
  </div>
</template>

<script lang="ts">
export default {
  props: {
    head: {
      default: "Header",
    },
    username: {
      default: "",
    },
    Loginded: {
      default: false,
    },
  },
  data: () => {
    return {
      text: "hello",
      menu: false,
    };
  },
  methods: {},
  async created() {}
};
</script>

<style>
</style>