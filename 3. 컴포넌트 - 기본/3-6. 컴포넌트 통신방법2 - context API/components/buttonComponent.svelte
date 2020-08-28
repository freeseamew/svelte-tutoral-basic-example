<script>
  import {createEventDispatcher} from 'svelte'

  const dispatch = createEventDispatcher()

  function handleIncrement(param) {
    dispatch('increment', {
    message: '값 증가 :' + param
    })
  }

  export let count
</script>

<button on:click={() => handleIncrement(10)} >
  increment count [{count}]
</button>