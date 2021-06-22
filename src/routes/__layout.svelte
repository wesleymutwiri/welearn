<script>
	import '../app.css';
	import Sidebar from '../components/Sidebar.svelte'
</script>

<div class="container">
	<Sidebar />
	<main>
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
	}
</style>
