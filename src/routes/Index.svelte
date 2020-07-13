<script>
	import Nav from "../components/Nav.svelte";
	import AthleteCards from "../components/AthleteCards.svelte"
	import TailwindCSS from "../components/TailwindCSS.svelte"
</script>

<svelte:head>
	<title>Tensight - Home of Asian Sports</title>
</svelte:head>

<TailwindCSS/>

<Nav page="/"/>

<main class="antialiased text-gray-900">
	<h1>The Global Home for Sports</h1>
	<iframe title="Athlete Gallery" class="airtable-embed" src="https://airtable.com/embed/shr4OV5llPWjRXZHW?backgroundColor=gray&viewControls=on" frameborder="0" onmousewheel="" width="100%" height="533" style="background: transparent; border: 1px solid #ccc;"></iframe>
	<div>
		<h2>New Athlete Cards</h2>
		<AthleteCards/>
	</div>
</main>

<style>
	main {
		text-align: center;
		padding: 1em;
		max-width: 240px;
		margin: 0 auto;
	}

	h1 {
		color: #859A00;
		font-size: 4em;
		font-weight: 100;
	}

	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	}
</style>