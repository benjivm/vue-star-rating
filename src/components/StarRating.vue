<template>
    <div
        @mouseleave="hoverRating = 0"
        class="flex items-center mx-auto"
    >
        <button
            v-for="star in totalStars"
            :key="star"
            @click="setRating(star)"
            @mouseover="hoverRating = star"
            class="focus:outline-none"
        >
            <svg
                viewBox="0 0 20 20"
                fill="currentColor"
                class="w-10 h-10 text-gray-300 -mx-1"
                :class="{ 'text-yellow-500' : (rating >= star && !hoverRating) || hoverRating >= star }"
            >
                <path d="M9.049 2.927c.3-.921 1.603-.921 1.902 0l1.07 3.292a1 1 0 00.95.69h3.462c.969 0 1.371 1.24.588 1.81l-2.8 2.034a1 1 0 00-.364 1.118l1.07 3.292c.3.921-.755 1.688-1.54 1.118l-2.8-2.034a1 1 0 00-1.175 0l-2.8 2.034c-.784.57-1.838-.197-1.539-1.118l1.07-3.292a1 1 0 00-.364-1.118L2.98 8.72c-.783-.57-.38-1.81.588-1.81h3.461a1 1 0 00.951-.69l1.07-3.292z" />
            </svg>
        </button>
    </div>
</template>

<script>
    import { ref } from 'vue';

    export default {
        props: {
            rating: {
                type: Number,
                required: true,
            },
            totalStars: {
                type: Number,
                required: false,
                default: 10
            }
        },

        emits: ['update:rating'],

        setup(props, context) {
            const hoverRating = ref(0);

            function setRating(value) {
                if (props.rating === value) {
                    return context.emit('update:rating', 0);
                }

                context.emit('update:rating', value);
            }

            return {
                hoverRating,
                setRating,
            };
        }
    };
</script>