<template>
  <div>
    <NuxtWelcome />
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
  async mounted() {
    console.log(await $fetch("/api/path"));
    console.log(await $fetch("/api/path/index"));
  },
});
</script>
