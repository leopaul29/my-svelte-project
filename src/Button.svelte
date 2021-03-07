<script>
  let count = 0;
  const handleClick = () => count += 1;

  $: plusDeux = count + 2;

  $: if (count > 5) {
    console.log(count);
  }

</script>


<button on:click={handleClick}>
  {count}
</button>

<p>{count} + 2 = {plusDeux}</p>

{#if count < 5}
  <p>Count est inférieur à 5.</p>
{:else if count < 10}
  <p>Count est inférieur à 10.</p>
{:else}
  <p>Count est supérieur ou égal à 10.</p>
{/if}
