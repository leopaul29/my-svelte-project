<script>
  const pokemons = [
    {
      name: 'Bulbizarre',
      type: 'plante'
    },
    {
      name: 'Salamèche',
      type: 'feu'
    },
    {
      name: 'Carapuce',
      type: 'eau'
    },
    {
      name: 'Pikachu',
      type: 'électrique'
    }
  ]
</script>

<ul>
  {#each pokemons as { name, type }, i}
    <li>{i + 1} : {name} | Type : {type.toUpperCase()}</li>
  {/each}
</ul>
