<script>
  import { count } from '../store'

  function handleIncrementCount() {
    count.update(count => count + 1)
  }
</script>

<button on:click={handleIncrementCount} >
  increment count [{$count}]
</button>