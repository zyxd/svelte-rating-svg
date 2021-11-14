Easy to use, run and install svelte component for building SVG star rating. You can use unlimited stars with fractional view. Component compatible with Server Side Rendering (SSR).


# Installation
```
npm install svelte-rating-svg
```

# Usage

```
<Rating/>

<script>
  import Rating from 'svelte-rating-svg'
</script>
```

# Properties

**value** - Value between 0 and 1__
**color** - Color of stars__
**max**  - Maximum number of stars__
**duration** - Filling of rating duration in seconds

# Examples

```<Rating value="0.5" color="green" max="3"/>```
```<Rating value="0.9" color="#AAA" duration="10000"/>```
```<Rating value="0.4321" max="1"/>```
