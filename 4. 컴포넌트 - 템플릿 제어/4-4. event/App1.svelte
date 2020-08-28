<script>
  function handleClick() {
    alert('no more alerts')
  }
</script>

<button on:click|once={handleClick}>클릭</button>