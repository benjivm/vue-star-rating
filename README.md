# Vue Star Rating

A simple star rating component built with Vue 3.

## Usage

Full source and dev server:

- Clone or download this repository to a directory of your choice
- Install dependencies: `npm i`
- Run dev server: `npm run dev`
- Build: `npm run build`

Component only:

- Copy the [StarRating.vue](https://github.com/benjivm/vue-star-rating/blob/master/src/components/StarRating.vue) component to your project.
- Replace all styles with your own (unless you are already using [Tailwind CSS](https://tailwindcss.com)).
- Use `v-model` to get the rating from the component, [like this](https://github.com/benjivm/vue-star-rating/blob/master/src/App.vue#L4).
- Optionally provide the [`stars` prop](https://github.com/benjivm/vue-star-rating/blob/master/src/App.vue#L5) if you'd like fewer (or more) stars, the default is 10.

### Notes

The star icon is from [Hero Icons](https://heroicons.com) and can be easily replaced with any SVG of your choice, refer to [`src/components/StarRating.vue`](https://github.com/benjivm/vue-star-rating/blob/master/src/components/StarRating.vue).
