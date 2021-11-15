<template>
    <div class="flex flex-col justify-center h-screen">
        <star-rating
            :rating="rating"
            @update:rating="rating = $event"
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
