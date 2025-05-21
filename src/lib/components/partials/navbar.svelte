<script>
	import NavbarLink from './navbar-link.svelte';
</script>

<nav class="bg-secondary text-secondary-foreground flex justify-between">
	<NavbarLink url="/" testo="Logo" />
	<div>
		<NavbarLink url="/contatti" testo="Contatti" />
		<NavbarLink url="/illustrazioni" testo="Illustrazioni" />
		<NavbarLink url="/motion" testo="Motion" />
		<NavbarLink url="/per-aziende" testo="Per Aziende" />
		<p>Per associazioni</p>
		<p>Brand Identity</p>
	</div>
</nav>
