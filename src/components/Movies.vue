<script setup >
import { useStore } from 'vuex'
import ListTitle from './ListTitle.vue'
import MoviesLIst from './MoviesLIst.vue';

 
const store=useStore()

const title=store.state.movie.name
const moviesData=store.state.movie.data
 
</script>

<template>
 <div class="w-full">
   <ListTitle :title="title"/>
    <MoviesLIst :data="moviesData"/>
    

 </div>

</template>