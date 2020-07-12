<script>
	import Nav from "../../components/Nav.svelte";
</script>

<Nav page="/blog/about-blog"/>

<style>
	main {
		padding: 1em;
		max-width: 240px;
		margin: 0 auto;
	}

	h1 {
		text-transform: uppercase;
		text-align: center;
		font-size: 4em;
		font-weight: 100;
	}

	@media (min-width: 640px) {
		main {
			max-width: none;
		}
    }
    
	ul {
		margin: 0 0 1em 0;
		line-height: 1.5;
    }

</style>

<svelte:head>
	<title>Blog</title>
</svelte:head>

<main>
    <h1>About the Blog</h1>

    <p>Before Tensight became an official publication, it started as a collection of random
	   musings deeply rooted in the conscience of a college senior, who was both hooked by the
	   stories of Asian(-American) athletes, and frustrated at the lack of coverage surrounding them.
	   As the idea grew slowly into a burning desire, that college senior stopped theorizing and
	   finally started writing. In case you’re curious, the name “Tensight” is a play on several things:
	</p>
	<ul>
		<li>
			The first is a pun on the Japanese term 天才, or “ten-sai”, meaning “genius, natural gift” — a 
			fitting phrase to describe the athletes in-detail.
	    </li>
		<li>
			If that’s not enough for you, the second is a play on the English term “foresight”, and that
			while people with “4-sight” may be able to see 4 steps into the future, “10-sight” will be
			able to see even further.
		</li>
	</ul>
	<p>I’ll hold for the applause.</p> 
	
</main>