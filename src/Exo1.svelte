<script>
  let checked = false;
</script>

<h2>Exo1</h2>
<input type="checkbox" name="checkbox" bind:checked={checked} />
{#if checked}
  <p>The checkbox is checked</p>
{/if}
