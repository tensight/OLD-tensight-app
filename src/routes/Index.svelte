<script>
	import Nav from "../components/Nav.svelte";
</script>

<svelte:head>
	<title>Tensight - Home of Asian Sports</title>
</svelte:head>

<Nav page="/"/>
<main>
	<h1>The Global Home for Sports</h1>
	<iframe title="Athlete Gallery" class="airtable-embed" src="https://airtable.com/embed/shr4OV5llPWjRXZHW?backgroundColor=gray&viewControls=on" frameborder="0" onmousewheel="" width="100%" height="533" style="background: transparent; border: 1px solid #ccc;"></iframe>
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