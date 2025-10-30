<template>
  <ParentComponent />
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import ParentComponent from "@/components/example4/ParentComponent.vue";

export default defineComponent({
  name: 'App',
  components: {
    ParentComponent
  }
});
</script>

<style>
</style>
