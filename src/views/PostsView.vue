<script setup>
import { RouterLink } from 'vue-router';
  const posts = [
    {id: '1', title: 'PHP'},
    {id: '2', title: 'Laravel'},
    {id: '3', title: 'Vue Js'},
    {id: '5', title: 'Livewire'},
  ]
</script>
<template>
  <div>
    <h1>All Posts</h1>
    <hr/>
    <div v-for="post in posts" :key="post.id">
      <h2><RouterLink :to="`posts/${post.id}`">{{ post.title }}</RouterLink></h2>  
    </div>
    
    
  </div>
</template>

<style>

</style>
