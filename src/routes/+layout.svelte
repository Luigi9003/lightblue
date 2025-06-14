<script>
	import '../app.css';
	import Navbar from '$lib/components/partials/navbar.svelte';
	import Footer from '$lib/components/partials/footer.svelte';
</script>

<div class="flex min-h-screen flex-col">
	<Navbar />

	<main class="mt-13 flex flex-grow items-center justify-center">
		<slot />
	</main>

	<Footer />
</div>
