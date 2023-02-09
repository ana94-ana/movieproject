<script setup >
import { useStore } from 'vuex'
import ListTitle from './ListTitle.vue'
import MovieList from './MovieList.vue'
import Watchlist from './watchlist.vue';
 
const store=useStore()

const title=store.state.movie.data
const moviesData=store.movie.data
 
</script>

<template>
 <div class="w-full">
    <MovieList :data="store.state.movie"/>
    <Watchlist/>

 </div>

</template>