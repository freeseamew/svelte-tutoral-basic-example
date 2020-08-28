<script>
let count = 0

function handleClick() {
	// 이벤트 코드
	count += 1
}

</script>

<button on:click={handleClick} >
	클릭수 { count } {count === 1 ? 'time' : 'times'}
</button>
