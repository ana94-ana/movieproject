<script setup>
import Movies from "./components/Movies.vue"
import Search from './components/Search.vue'
import watchlist from './components/WatchS.vue'
import { useStore } from 'vuex'
import ListTitle from "./components/ListTitle.vue"



</script>

<template>
  
  <div>
   <Search/>
   <Movies />
   <watchlist />
  </div>
</template>