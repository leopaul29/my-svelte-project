<script>
	export let name;
	import Exo1 from './Exo1.svelte'
	import Exo2 from './Exo2.svelte'
	import Bio from './Bio.svelte'
	import Button from './Button.svelte'
	import SuperButton from './SuperButton.svelte'
	import Fibonacci from './Fibonacci.svelte'
	import Liste from './Liste.svelte'
	import Pokedex from './Pokedex.svelte'
</script>

<main>
	<h1>Hello {name}!</h1>
	<p>Visit the <a href="https://svelte.dev/tutorial">Svelte tutorial</a> to learn how to build Svelte apps.</p>
</main>

<Exo1/>
<Exo2/>
<Bio/>
<Button/>
<SuperButton/>
<Fibonacci/>
<Liste/>
<Pokedex/>

<style>
	main {
		text-align: center;
		padding: 1em;
		max-width: 240px;
		margin: 0 auto;
	}

	h1 {
		color: #ff3e00;
		text-transform: uppercase;
		font-size: 4em;
		font-weight: 100;
	}

	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	}
</style>