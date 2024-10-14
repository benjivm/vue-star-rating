<script setup>
import { ref } from 'vue';
import StarRating from './components/StarRating.vue';

const rating = ref(0);
</script>

<template>
    <div class="flex h-screen flex-col justify-center">
        <StarRating v-model="rating" />

        <div class="mx-auto p-3 font-mono font-black">Rating: {{ rating }}</div>
    </div>
</template>