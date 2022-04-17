<script>
  let count = 0

  function incrementCount() {
    count += 1
  }
  $: doubled = count * 2
</script>

<div>
  <h2>Reactivity</h2>
  <button on:click={incrementCount}>
    Clicked {count}
    {count === 1 ? 'time' : 'times'}
  </button>
  <p>{count} doubled is {doubled}</p>
</div>
