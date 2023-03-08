
<!-- routing in svelte(kit) is based on a batteries included structure, so there isn't a reason to use a router. this page is located at / and pants is located at /pants -->

<script>
	import Styleddiv from './styleddiv.svelte';
	import "./main.css";
	let name = 'world';
	function parentToggle(value) { 
		console.log('inside parentToggle: ', value)
	}
</script>

<div class="main">
	<h1>Hello {name}!</h1>
	<Styleddiv toggle={parentToggle}/>

	<h1>Welcome to SvelteKit</h1>
	<p>Visit <a href="https://kit.svelte.dev">kit.svelte.dev</a> to read the documentation</p>

	<a href="/pants">Secondary Page</a>
</div>
