<script>
  import { getContext } from 'svelte'
  // export let count

  let handleIncrementCount = getContext('incrementCount')
  let count = getContext('count')
</script>

<button on:click={handleIncrementCount} >
  increment count [{count}]
</button>