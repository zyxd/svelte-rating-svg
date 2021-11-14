Easy to use, run and install svelte component for building SVG star rating. You can use unlimited stars with fractional view. Component compatible with Server Side Rendering (SSR).


## Installation
```
npm install svelte-rating-svg
```

## Usage

```
<Rating/>

<script>
  import Rating from 'svelte-rating-svg'
</script>
```
or you can use direct link to generate SVG:
https://svelte-rating-svg.vercel.app/rating-[value]-[max]-[color].svg

## Properties

**value** - Value between 0 and 1</br>
**color** - Color of stars</br>
**max**  - Maximum number of stars</br>
**duration** - Filling of rating duration in seconds

## Examples

```<Rating value="0.5" color="green" max="3"/>```  ![rating-0.5-3-green.svg](https://svelte-rating-svg.vercel.app/rating-0.5-3-green.svg) </br>
```<Rating value="0.9" color="#AAA" duration="10000"/>```  ![rating-0.9-5-%23AAA.svg](https://svelte-rating-svg.vercel.app/rating-0.9-5-%23AAA.svg)</br>
```<Rating value="0.4321" max="1"/>```  ![rating-0.4321-1-red.svg](https://svelte-rating-svg.vercel.app/rating-0.4321-1-red.svg) </br>
```https://svelte-rating-svg.vercel.app/rating-0.5-4-blue.svg``` ![rating-0.5-4-blue.svg](https://svelte-rating-svg.vercel.app/rating-0.5-4-blue.svg) </br>

