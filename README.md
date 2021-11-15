# Vue Star Rating

A simple star rating component built with Vue 3.

## Usage

Full source and dev server:

- Clone or download this repository to a directory of your choice
- Install dependencies: `npm i`
- Run dev server: `npm run dev`
- Build: `npm run build`

Component only:

- Copy the [StarRating.vue](https://github.com/benjivm/vue-star-rating/blob/master/src/components/StarRating.vue) component to your project
- Replace all styles with your own (unless you are already using [Tailwind CSS](https://tailwindcss.com))
- Provide the `rating` prop and listen for the [`@update:rating`](https://v3.vuejs.org/guide/component-custom-events.html) event, [like this](https://github.com/benjivm/vue-star-rating/blob/9a212980e1929a619eea465e584a0d99e49c9f0b/src/App.vue#L3)

### Notes

The star icon is from [Hero Icons](https://heroicons.com) and can be easily replaced with any SVG of your choice, refer to `src/components/StarRating.vue`.
