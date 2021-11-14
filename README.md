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

## Properties

**value** - Value between 0 and 1</br>
**color** - Color of stars</br>
**max**  - Maximum number of stars</br>
**duration** - Filling of rating duration in seconds

## Examples

```<Rating value="0.5" color="green" max="3"/>``` </br>
data:image/svg+xml; <svg width="96" height="32" viewBox="0 0 96 32" class="svelte-1bvf986"><defs><mask id="perc-706231"><rect x="0" y="0" width="100%" height="100%" fill="#fff"></rect><rect x="50%" y="0" width="100%" height="100%" fill="#222"></rect></mask><symbol viewBox="0 0 32 32" id="star-706231"><path d="M31.547 12a.848.848 0 00-.677-.577l-9.427-1.376-4.224-8.532a.847.847 0 00-1.516 0l-4.218 8.534-9.427 1.355a.847.847 0 00-.467 1.467l6.823 6.664-1.612 9.375a.847.847 0 001.23.893l8.428-4.434 8.432 4.432a.847.847 0 001.229-.894l-1.615-9.373 6.822-6.665a.845.845 0 00.214-.869z"></path></symbol><symbol viewBox="0 0 96 32" id="stars-706231"><use xlink:href="#star-706231" x="-32" y="0"></use><use xlink:href="#star-706231" x="0" y="0"></use><use xlink:href="#star-706231" x="32" y="0"></use></symbol></defs><use xlink:href="#stars-706231" fill="green" stroke="black" mask="url(#perc-706231)"></use></svg>
```<Rating value="0.9" color="#AAA" duration="10000"/>``` </br>
```<Rating value="0.4321" max="1"/>``` </br>
