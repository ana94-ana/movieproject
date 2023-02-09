<script setup >
import { useStore } from 'vuex'
import ListTitle from './ListTitle.vue'
import MovieList from './MovieList.vue'
import Watchlist from './watchlist.vue'

const store=useStore()

const title=store.state.watch.data
const data=store.state.watch.data

</script>

<template>
<div class="w-full ">
    <ListTitle :title="title"/>
    <Watchlist :data="data"/>

</div>

</template>