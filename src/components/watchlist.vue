<script >
export default{ 
    props: {
        data:{type: Array}
     }
    }
 
</script>

<template>
 <div class="w-full" > 
    <ul>
        <li v-for=" name in data" :key="name.id">{{ name.id }} -{{ name.name }} -{{ name.url }}-{{ name.description }}-{{ name.cover }}</li>
    </ul>
 </div>

</template>