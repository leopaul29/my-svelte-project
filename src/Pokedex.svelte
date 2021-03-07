<script>
  const getPokemon = async () => {
    const res = await fetch('https://pokeapi.co/api/v2/pokemon?limit=151')
    const json = await res.json()

    return json.results
  }

  let pokemons = getPokemon()
</script>

{#await pokemons}
  <p>Les pokemons arrivent !!!</p>
{:then pokemons}
  <ul>
    {#each pokemons as { name }}
      <li>{name}</li>
    {/each}
  </ul>
{/await}
