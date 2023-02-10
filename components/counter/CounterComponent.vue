<script lang="ts" setup>
const localCounter = ref<number>(0);
const doubledLocalCounter = computed<number>(() => localCounter.value * 2);
</script>

<template>
  <fieldset>
    <legend>Counter</legend>
    <button @click.prevent="localCounter++">
      Local: {{ localCounter }} * 2 = {{ doubledLocalCounter }}
    </button>
  </fieldset>
</template>
