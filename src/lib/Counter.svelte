<script>
  let count = $state(parseInt(localStorage.getItem('count')) || 0);

  const increment = () => {
    count += 1;
    localStorage.setItem('count', count);
  }
</script>

<button class="button" onclick={increment}>
  count is {count}
</button>
