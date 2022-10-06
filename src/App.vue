<script setup>
import { ref, onMounted } from "vue";

let tableau = ref([2, 1]);

onMounted(() => tableau.value.sort((a, b) => (a < b ? 0 : 1)));
</script>

<template>
  <h1>Utilisé-je Firefox ?</h1>
  <br />
  <h2>{{ tableau[0] < tableau[1] ? "Oui" : "Non" }}</h2>
</template>
