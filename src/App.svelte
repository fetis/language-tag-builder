<script>
	import Test from './Test.svelte';
	import svelte from 'svelte/compiler';

	export const time = Date.now();
</script>

<main>
	<h1>BCP 47 Language tag builder</h1>
	{ time }

	<Test />
<!--	{#await promise}-->
<!--		-->
<!--	{/await}}-->
	<p>
		Generated with Svelte v{svelte.VERSION}
	</p>
</main>

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


