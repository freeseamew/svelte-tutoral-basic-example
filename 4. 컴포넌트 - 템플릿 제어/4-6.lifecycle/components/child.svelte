<script>
  import { onMount, onDestroy, beforeUpdate, afterUpdate, tick } from 'svelte'

  onMount(async() => {
    console.log('child onMount')
  })

  onDestroy(async() => {
    console.log('child onDestroy')
  })

  beforeUpdate(async() => {
    console.log('the component is about to update');
    await tick()
    console.log('the component just updated');  
  })

  afterUpdate(async() => {
    console.log('child afterUpdate')
  })
</script>