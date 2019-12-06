<script>
  let count = 0;

  function handleClick() {
    count += 1;
  }

  function handleDoubleClick() {
      count = 0;
  }
</script>

<button on:click={handleClick} on:dblclick|preventDefault={handleDoubleClick}>
  Clicked {count} {count === 1 ? 'time' : 'times'}
</button>
