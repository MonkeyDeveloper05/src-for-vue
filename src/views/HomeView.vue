<script setup lang="ts">
  type ToDo = {
    id: number,
    title: string,
    completed: boolean,
  } 

  const list: ToDo[] = [
    {
      id: 1,
      title: "ciao",
      completed: false,
    },
    {
      id: 2,
      title: "hello",
      completed: false,
    },
    {
      id: 3,
      title: "hola",
      completed: true,
    }
]
</script>

<template>
  <main class="container mt-4">
    <li v-for="item in list" :key="item.id">
      {{ item.title }}
    </li>
  </main>
</template>
