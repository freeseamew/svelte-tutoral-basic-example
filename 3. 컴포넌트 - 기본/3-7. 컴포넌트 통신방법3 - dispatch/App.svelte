<script>
  import { setContext } from 'svelte'
  import PanelComponent from './components/panelComponent.svelte'

  let count = 10

  function incrementCount(event) {
    count ++
  }

  setContext('incrementCount', incrementCount)
  setContext('count', count)
</script>

<PanelComponent {count} />