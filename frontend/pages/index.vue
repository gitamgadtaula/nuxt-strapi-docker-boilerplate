<template>
  <div>
    <h1>Logged in as: {{ user?.email }}</h1>
  </div>
</template>

<script setup>
const user = useStrapiUser();
</script>

<style>
</style>