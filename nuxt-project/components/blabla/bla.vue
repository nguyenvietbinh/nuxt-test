<script setup>
async function submit() {
  const res = await $fetch('/api/submit', {
    method: 'post',
    body: JSON.stringify({ message: 'tell me a joke' })
  })
  console.log(res);
}
</script>

<template>
  <button @click="submit">blabla</button>
</template>