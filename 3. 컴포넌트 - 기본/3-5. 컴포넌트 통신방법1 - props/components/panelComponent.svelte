<script>
  import ButtonComponent from './buttonComponent.svelte'

  export let count
  export let incrementCount
</script>

<div class="penal">
  <h1>{count}</h1>

  <ButtonComponent {incrementCount} />
</div>

<style>
  .penal {
    padding: 20px;
    display:flex;
    flex-direction: column;
    justify-items: center;
    justify-content: space-around;
    align-items: center;
    height: 500px;
    width:400px;
    background: #e2e2e2;
    border: 1px solid #777777;
  }
</style>