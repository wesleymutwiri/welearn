<script>
	import Header from '$lib/Header/index.svelte';
	import '../app.css';
	import Sidebar from '../components/Sidebar.svelte'
</script>

<div class="container">
	<Sidebar />
	<main>
		<Header />
		<slot />
	</main>
</div>
	
	<footer>
		
	</footer>

<style>
	.container {
		display: flex;
	}
	main {
		flex: 1;
		display: flex;
		flex-direction: column;
		padding: 1rem;
		width: 100%;
		max-width: 1024px;
		margin: 0 auto;
		box-sizing: border-box;
	}
</style>
