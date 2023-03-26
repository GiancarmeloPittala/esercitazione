<template>
    <nuxtLink :to="to" class="text-gray-400 hover:text-black pb-2" v-bind="$attrs">
        <slot>
            {{text}}
        </slot>
        </nuxtLink>
</template>
<script>
export default {
    inheritAttrs:false 
}
</script>

<script setup>
defineProps ({
    to:{
        type:string
     },
     text: {
        type:string,
        required:true
     }})
</script>