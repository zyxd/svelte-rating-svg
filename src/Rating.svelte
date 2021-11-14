<svg width={width_total} height={height} viewBox={`0 0 ${width_total} ${height}`} xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink">
  <defs>
		<mask id={`perc-${random}`}>
      <rect x="0" y="0" width="100%" height="100%" fill="#fff" />
      <rect x={`${$value_tweened * 100}%`} y="0" width="100%" height="100%" fill="#222" />
    </mask>

    <symbol viewBox={`0 0 ${width} ${height}`} id={`star-${random}`}>
      <path d="M31.547 12a.848.848 0 00-.677-.577l-9.427-1.376-4.224-8.532a.847.847 0 00-1.516 0l-4.218 8.534-9.427 1.355a.847.847 0 00-.467 1.467l6.823 6.664-1.612 9.375a.847.847 0 001.23.893l8.428-4.434 8.432 4.432a.847.847 0 001.229-.894l-1.615-9.373 6.822-6.665a.845.845 0 00.214-.869z" />
    </symbol>
		
    <symbol viewBox={`0 0 ${width_total} ${height}`} id={`stars-${random}`}>
			{#each {length: max} as _, index}
				<use xlink:href={`#star-${random}`} x={get_offset(width, max, index)} y="0"></use>
			{/each}
    </symbol>
  </defs>

  <use xlink:href={`#stars-${random}`} fill={color} stroke="black" mask={`url(#perc-${random})`}></use>
</svg>

<script>
	import { tweened } from 'svelte/motion'
	import { cubicOut } from 'svelte/easing'
	
	export let max = 5
	export let value = 0
	export let color = 'red'
	export let duration = 1000

	const random = Math.floor(Math.random() * 1000000)
	
	const value_tweened = tweened(value, {
		duration,
		easing: cubicOut
	})
	
	const width = 32
	const height = 32
	const get_offset = (w, m, v) => (v * w) - (((m * w) - w) / 2)
	
	$: value_tweened.set(parseFloat(value) || 0)
	$: width_total = width * max
</script>

<style>
	svg {
		width: 100%;
		height: 100%;
	}
</style>