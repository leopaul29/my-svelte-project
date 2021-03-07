<script>
  import marked from 'marked'
  let name = 'Antho'
  let checked = false
  let value = `
  # Mon titre

  * pomme
  * poire
  * pêche
  `
</script>

<input type="text" bind:value={name}>

<h1>Hello {name}</h1>

<label>
  <input type=checkbox bind:checked={checked}>
  Accépter de donner toutes mes données personnelles pour pouvoir regarder des vidéos de chats.
</label>

{#if checked}
  <p>Merci de ne pas avoir lu toutes les petites closes.</p>
{/if}

<textarea cols="30" rows="10" bind:value={value}></textarea>

{@html marked(value)}
