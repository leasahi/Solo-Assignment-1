<script setup>
import {computed, ref} from 'vue'

const count = ref(0)
const triple = computed(() => count.value*3)
</script>

<template>
  <h1>
    Count: {{ count }}
  </h1>
  <h2>
    Triple of Count: {{ triple }}
  </h2>
  <div class="buttons">
    <button type="button" @click="count--">
      <h2>
        -
      </h2>
    </button>
    <button type="button" @click="count++">
      <h2>
        +
      </h2>
    </button>
  </div>

</template>

<style scoped>

</style>