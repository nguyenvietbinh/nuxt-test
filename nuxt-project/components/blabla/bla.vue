<script setup>
async function submit() {
  const res = await $fetch('/api/submit', {
    method: 'post',
    body: JSON.stringify({ message: 'hello' })
  })
  console.log(res);
}
</script>

<template>
  <button @click="submit">blabla</button>
</template>