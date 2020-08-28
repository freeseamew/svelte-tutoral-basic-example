<script>
	let value = '안녕하세요. svelte 강좌 입니다.'
	let active = false
</script>

<p> {value} </p>
<input type="checkbox" bind:checked={active} /> {active}
