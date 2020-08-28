<script>
	import { fade, blur, fly, slide, scale, draw } from 'svelte/transition';
	
	let condition = false
	
</script>

<label>
	<input type="checkbox" bind:checked={condition} /> 
	효과 보기
</label>


{#if condition}
	<div transition:blur="{{delay: 200, duration: 300, opacity: 1, amount: 5}}">
		transiton 예제
	</div>
{/if}