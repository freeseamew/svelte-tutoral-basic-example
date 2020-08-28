<script>
	import { draw } from 'svelte/transition';
	import { quintOut } from 'svelte/easing';
	
	let condition = false
</script>

<label>
	<input type="checkbox" bind:checked={condition} /> 
	효과 보기
</label>

<svg viewBox="0 0 5 5" xmlns="http://www.w3.org/2000/svg">
	{#if condition}
		<path transition:draw="{{duration: 5000, delay: 500, easing: quintOut}}"
					d="M2 1 h1 v1 h1 v1 h-1 v1 h-1 v-1 h-1 v-1 h1 z"
					fill="none"
					stroke="cornflowerblue"
					stroke-width="0.1px"
					stroke-linejoin="round"
		/>
	{/if}
</svg>