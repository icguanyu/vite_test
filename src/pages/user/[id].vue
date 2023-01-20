<script setup>
import { onMounted, ref } from "@vue/runtime-core";
import { useRoute } from "vue-router";
const id = ref("");
const route = useRoute();

onMounted(() => {
  id.value = route.params.id;
});
</script>

<template>
  <div>user id: {{ id }}</div>
</template>
