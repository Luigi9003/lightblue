<script>
	import NavbarLink from './navbar-link.svelte';
	import { base, assets } from '$app/paths';
</script>

<nav class="bg-secondary text-secondary-foreground flex justify-between">
	<a href="{base}/">
		<img src="{assets}/immagini/lightblue-logo.svg" alt="Logo" class="h-10" />
	</a>
	<div class="flex items-center gap-2">
		<NavbarLink url="/motion" testo="Motion" />
		<p>Brand Identity</p>
		<NavbarLink url="/per-aziende" testo="Per Aziende" />
		<NavbarLink url="/per-associazioni" testo="Per Associazioni" />
		<NavbarLink url="/illustrazioni" testo="Illustrazioni" />
		<NavbarLink url="/contatti" testo="Contatti" />
	</div>
</nav>
