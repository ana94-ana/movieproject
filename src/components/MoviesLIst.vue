<script setup>
import ActionButton from './ActionButton.vue'
defineProps({
    data:{type:Array, required:true},
    action:{type:Boolean}
    
})

</script>

<template>

    <ul >
        <li class="max-w-sm bg-white border border-gray-200 rounded-lg shadow dark:bg-gray-800 dark:border-gray-700"
         v-for=" title in data" :key="title.id">
         <span>{{ title.id }} -{{ title.name }} -{{ title.description }}-{{ title.cover }}</span>
        <ActionButton :tomovie="action" :id="item.id"/>
    </li>
    </ul>

</template>