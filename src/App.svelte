<script>
	export let name;
	let svelteLogo = "https://arepa.s3.amazonaws/svelte-logo.png"
</script>

<main>
	<h1>Hello {name}!</h1>
	<p>FullStack Software Engineer</p>
	<img src={svelteLogo} alt="Svelte">
</main>

<style>
	:global(body){
		background-color: #f2eee2;
		color: #0084f6
	}
	:global(:root){
		--theme-color: purple;
	}

	p{
		color: var(--theme-color);
		font-size: 24px;
	}
	main {
		text-align: center;
		padding: 1em;
		max-width: 240px;
		margin: 0 auto;
	}
	
	main img {
		height: 30%;
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