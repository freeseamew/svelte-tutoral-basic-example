<script>
  import PanelComponent from './components/panelComponent.svelte'

  let count = 10

  function incrementCount(event) {
    // count = count + 1
    console.log(event.detail.message)
    count ++
  }
</script>

<PanelComponent {count} on:increment={incrementCount}/>