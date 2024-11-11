<script setup>
import { ref } from 'vue'
const qmode = ref(true)
defineProps({data: Object})
</script>
<template>
  <div :class="qmode ? 'divq' : 'divq diva'" @click="qmode = !qmode">
    {{ qmode ? data.question : data.answer }}
  </div>
</template>
