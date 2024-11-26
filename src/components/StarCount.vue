<script setup>
 defineProps({
     rating: {
         type: Number,
         default: 0
     },
     reviews: {
         type: String,
         default: '0'
     }
 })
</script>

<template>
    <div class="flex gap-4 items-center">
        <div class="flex gap-1">
            <template v-for="index in Math.ceil(rating)" :key="index" >
                <i class="bi bi-star-fill text-yellow-400"></i>
            </template>
        </div>
        <span class="text-xs text-gray-600">
            {{rating}}/5 ({{reviews}} reviews)
        </span>
    </div>
</template>

<style scoped></style>