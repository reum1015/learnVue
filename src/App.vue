<template>
  <div class="container mt-5">
    <div class="logo_wrapper">
      <img alt="Vue logo" src="./assets/logo.png">
    </div>
    <div class="notification is-success">
      <button class="delete"></button>
      Primar lorem ipsum dolor sit amet, consectetur adipiscing elit lorem ipsum
      dolor. <strong>Pellentesque risus mi</strong>, tempus quis placerat ut, porta
      nec nulla. Vestibulum rhoncus ac ex sit amet fringilla. Nullam gravida purus
      diam, et dictum <a>felis venenatis</a> efficitur.
    </div>

    <input class="input" ref="my-input">

  </div>
</template>

<script setup>
import { useTemplateRef, onMounted } from 'vue'

const input = useTemplateRef('my-input')

onMounted(() => {
  input.value.focus()
})

</script>

<style>
.logo_wrapper{
  display: flex;
  justify-content: center;
  margin-bottom: 4rem;
}
</style>
