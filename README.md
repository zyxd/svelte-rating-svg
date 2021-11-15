<a href="https://svelte-rating-svg.vercel.app">
  <img width="100%" src="https://svelte-rating-svg.vercel.app/rating-0.70-12-orange.svg">
</a>

#### Easy to use, run and install [Svelte](https://github.com/sveltejs/svelte) component for building SVG stars-rating. It can be used to make unlimited stars with fractional rating and any colors. Component compatible with Server Side Rendering (SSR).


## Installation
```bash
npm install svelte-rating-svg
```

## Usage

```svelte
<script>
  import Rating from 'svelte-rating-svg'
</script>

<Rating value="0.25"/>
```

## Properties

| Property | Description | Type | Default |
| --- | --- | --- | --- |
| **value** | Value between 0 and 1 | Number | 0 |
| **color** | Color of stars | String | red |
| **max** | Maximum number of stars | Number | 5 |
| **duration** | Transition duration in milliseconds | Number | 1000 |

## Examples

| Code | Result |
| --- | --- |
| `<Rating value="0.5" color="green" max="3"/>` | ![rating-0.5-3-green.svg](https://svelte-rating-svg.vercel.app/rating-0.5-3-green.svg) |
| `<Rating value="0.9" color="#AAA" duration="10000"/>` | ![rating-0.9-5-#AAA.svg](https://svelte-rating-svg.vercel.app/rating-0.9-5-%23AAA.svg) |
| `<Rating value="0.4321" max="1"/>` | ![rating-0.4321-1-red.svg](https://svelte-rating-svg.vercel.app/rating-0.4321-1-red.svg) |
