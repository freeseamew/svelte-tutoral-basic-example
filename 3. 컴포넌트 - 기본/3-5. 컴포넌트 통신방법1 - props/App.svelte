
<script>
  import PanelComponent from './components/panelComponent.svelte'

  let count = 10

  function incrementCount() {
    // count = count + 1
    count ++
  }

</script>

<PanelComponent {count} {incrementCount} />