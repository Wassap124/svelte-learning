<script>
  let count = 0;
  $: squaredCount = count ** 2;

  function handleClick() {
    count += 1;
  }

  // This will trigger every time count changes. i.e - we could write
  // The condition like this instead of checking it in the `handleClick` function
  $: if (count > 10) {
    count = 0;
  }
</script>

<button on:click={handleClick}>
  Clicked {count} {count === 1 ? 'time' : 'times'}
</button>
<p>The times that the buttons was clicked - squared - is: {squaredCount}</p>
