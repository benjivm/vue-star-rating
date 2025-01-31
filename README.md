# Vue Star Rating

A simple star rating component built with Vue 3.

## Usage

### Full source and preview/dev server:

- Clone or download this repository to a directory of your choice
- Install dependencies: `npm i`
- Build: `npm run build` (or skip this and the next step and just run the dev server: `npm run dev`)
- Run preview: `npm run serve`

### Component

- Copy the [StarRating.vue](https://github.com/benjivm/vue-star-rating/blob/master/src/components/StarRating.vue) component to your project.
- Replace all styles with your own (unless you are already using [Tailwind CSS](https://tailwindcss.com)).
- Use `v-model` to get the rating from the component, [like this](https://github.com/benjivm/vue-star-rating/blob/master/src/App.vue#L10).
- Optionally provide the `stars` prop like fewer (or more) stars, the default is 10.

### Notes

The star icon is from [Hero Icons](https://heroicons.com) and can be easily replaced with any SVG of your choice, refer to [`src/components/StarRating.vue`](https://github.com/benjivm/vue-star-rating/blob/master/src/components/StarRating.vue).
