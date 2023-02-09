<script setup>
import { propsToAttrMap } from '@vue/shared';
import { watch } from 'vue';
import { useStore } from 'vuex';

defineProps({
    tocart:{type:Boolean, required:false, default:true},
    id:{type:Number,required:true}
})

const store=useStore()

function addWatch(){
store.commit.apply("addItemVideo", props.id)
}

function removevideo(){
    store.commit.apply("removeItemWatch", props.id)
}

</script>

<template>
<button v-if="tocart" @click.prevent="addWatch"  class="text-gray-900 bg-gradient-to-r from-teal-200 to-lime-200 hover:bg-gradient-to-l hover:from-teal-200 hover:to-lime-200 focus:ring-4 focus:outline-none focus:ring-lime-200 dark:focus:ring-teal-700 font-medium rounded-lg text-sm px-5 py-2.5 text-center mr-2 mb-2">add</button>
<button v-else @click.prevent="removevideo" class="text-white bg-gradient-to-br from-pink-500 to-orange-400 hover:bg-gradient-to-bl focus:ring-4 focus:outline-none focus:ring-pink-200 dark:focus:ring-pink-800 font-medium rounded-lg text-sm px-5 py-2.5 text-center mr-2 mb-2">delete</button>

</template>