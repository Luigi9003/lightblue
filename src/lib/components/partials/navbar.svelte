<script>
	import NavbarLink from './navbar-link.svelte';
	import { base, assets } from '$app/paths';
</script>

<div class="bg-secondary text-secondary-foreground">
	<nav class="mx-auto flex justify-between px-2 py-1">
		<a href="{base}/" class="shrink-0">
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
</div>
