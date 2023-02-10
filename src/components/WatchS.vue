<script setup >
import { useStore } from 'vuex'
import ListTitle from './ListTitle.vue'
import MoviesLIst from './MoviesLIst.vue';


const store=useStore()

const title=store.state.watch.name
const data=store.state.watch.data

</script>

<template>
<div class="w-full ">
    <ListTitle :title="title"/> 
    <MoviesLIst :data="data"/>

</div>

</template>