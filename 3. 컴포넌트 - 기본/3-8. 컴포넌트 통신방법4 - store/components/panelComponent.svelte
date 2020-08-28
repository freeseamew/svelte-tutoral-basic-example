<script>
  import ButtonComponent from './buttonComponent.svelte'

  import { count } from '../store'
</script>

<div class="penal">
  <h1>{$count}</h1>
  
  <ButtonComponent  />
  
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