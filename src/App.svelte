<script lang="ts">
    import Nested from './Nested.svelte'
    export let  name:string,test:number
</script>

<main>
	<h1>Hello {name}! {test}</h1>
    <p>Svelte using export statement to pass through props</p>
    <Nested/>
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