<template>
    <div class="flex flex-col justify-center h-screen">
        <star-rating
            v-model="rating"
            :stars="10"
        />

        <div class="mx-auto p-3">
            Rating: {{ rating }}
        </div>
    </div>
</template>

<script setup>
    import { ref } from 'vue';
    import StarRating from './components/StarRating.vue';

    const rating = ref(0);
</script>
