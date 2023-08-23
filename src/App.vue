<script setup>
import { reactive, ref } from "vue";

// component logic
// declare some reactive state here.
const age = reactive({
  myAge: 28,
});
const message = ref("Hey There, Asfia");
const titleClass = ref("title");
const buttonTitle = ref('Click me!');
const textColor = ref('violet');
const isActive = ref(false);
</script>

<template>
  <h1>{{ message.split("").reverse().join("") }}</h1> <br>
  <p style="margin: 20px">My age is is : {{ age.myAge }}</p> <br>
  <!-- Attribute Binding -->
  <!-- 1. Class Attribute -->
  <h1 :class="titleClass">My color is green</h1> <br>
  <!-- 2. Title Attribute -->
  <button :title="buttonTitle">Hover me</button> <br>
  <!-- 3. Binding Inline Styles -->
  <p :style="{ color: textColor }">My color is violet</p> <br>
  <!-- 4. Conditional Attribute Binding -->
  <button :class="{ 'active': isActive }">Toggle</button> <br>
  <!-- 5. Binding Multiple Attributes -->
  <button :class="{ 'active': isActive }" :style="{ backgroundColor: isActive ? 'blue' : 'pink' }">Toggle</button> <br>
</template>

<style>
.title {
  color: green;
}
</style>
