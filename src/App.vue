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

<script>
    import StarRating from './components/StarRating.vue';

    export default {
        components: {
            StarRating
        },

        data() {
            return {
                rating: 0
            };
        }
    };
</script>
