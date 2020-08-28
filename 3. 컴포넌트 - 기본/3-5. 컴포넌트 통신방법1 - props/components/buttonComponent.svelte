<script>
  export let count
  export let incrementCount
</script>

<button on:click={incrementCount} >
  increment count [{count}]
</button>