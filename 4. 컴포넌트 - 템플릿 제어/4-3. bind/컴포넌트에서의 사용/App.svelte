<script>
	import CountComp from './countComp.svelte'
	
	let viewValue = 0
</script>

<h2>{viewValue}</h2>

<CountComp bind:count={viewValue} />