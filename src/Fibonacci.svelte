<script>
  let fibonacci = [0, 1, 1, 2, 3];
  const handleClick = () => {
    // fibonacci.push(fibonacci[fibonacci.length - 1] + fibonacci[fibonacci.length - 2])
    const suivant = fibonacci[fibonacci.length - 1] + fibonacci[fibonacci.length - 2]
    fibonacci = [...fibonacci, suivant]
  }

</script>

<br>
<button on:click={handleClick}>
  Fibonacci
</button>

<p>{fibonacci.join(' | ')}</p>
