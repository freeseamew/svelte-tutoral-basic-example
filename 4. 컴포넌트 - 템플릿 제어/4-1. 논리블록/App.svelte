<script>
  let login = true

  function handleClick() {
    login = !login // logic 값이 true면 false, 그리고 false true 만들어 주는 간다한 코드입니다. 
  }
</script>

<button on:click={handleClick} >호출</button>

{#if login === true}
  <p> 현재 login은 참입니다. </p> 
{:else}
  <p> 현재 login은 거짓입니다. </p> 
{/if}