<script>
	let name = 'Alon';
    import Nested from './Nested.svelte';
    let count = 0;

	function incrementCount() {
		count += 1;
	}
</script>

<style>
	p {
		color: purple;
		font-family: 'Comic Sans MS', cursive;
		font-size: 2em;
	}
</style>

<h1>Hello {name.toUpperCase()}</h1>

<p>This is a paragraph.</p>
<Nested answer={"4222"}/>
<Nested/>
<Nested answer={"44432"}/>
<Nested answer={"4342"}/>
<Nested answer={"432"}/>
<Nested answer={"342"}/>

<button on:click={incrementCount}>
	Clicked {count} {count === 1 ? 'time' : 'times'}
</button>