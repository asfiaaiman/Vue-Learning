<script setup>
import { reactive, ref } from 'vue'

// component logic
// declare some reactive state here.
  const age = reactive({
    myAge: 28
  })
  const message = ref('Hey There, Asfia')
</script>

<template>
  <h1>{{ message.split('').reverse().join('') }}</h1>
  <p style="margin: 20px;">
    My age is is : {{ age.myAge }}
  </p>
</template>