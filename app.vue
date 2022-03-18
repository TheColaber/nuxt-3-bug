<template>
  <div>
    <NuxtWelcome />
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
  async setup() {
    console.log(await $fetch("/api/data"));
  },
});
</script>
