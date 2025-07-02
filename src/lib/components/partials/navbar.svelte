<script lang="ts">
	import NavbarLink from './navbar-link.svelte';
	import { base, assets } from '$app/paths';
	import * as Sheet from '$lib/components/ui/sheet/index.js';
	import MobileMenuLink from './mobile-menu-link.svelte';
	import { onNavigate } from '$app/navigation';
	import SquareMenu from '@lucide/svelte/icons/square-menu';

	type Link = {
		url: string;
		testo: string;
	};

	const links: Array<Link> = [
		{ url: '/motion', testo: 'Motion' },
		{ url: '/motion', testo: 'Brand Identity' },
		{ url: '/per-aziende', testo: 'Per Aziende' },
		{ url: '/per-associazioni', testo: 'Per Associazioni' },
		{ url: '/illustrazioni', testo: 'Illustrazioni' },
		{ url: '/contatti', testo: 'Contatti' }
	];

	let isOpen = $state(false);

	onNavigate(() => {
		isOpen = false;
	});
</script>

<div class="bg-secondary text-secondary-foreground fixed top-0 z-50 w-full">
	<nav class="mx-auto flex max-w-[95vw] justify-between px-2 py-2">
		<a href="{base}/" class="shrink-0">
			<img src="{assets}/immagini/lightblue-logo.svg" alt="Logo" class="h-9" />
		</a>
		<div class="hidden items-center gap-2 md:flex">
			{#each links as link}
				<NavbarLink url={link.url} testo={link.testo} />
			{/each}
		</div>

		<Sheet.Root bind:open={isOpen}>
			<Sheet.Trigger class="block md:hidden"><SquareMenu /></Sheet.Trigger>
			<Sheet.Content class="bg-secondary text-secondary-foreground w-screen md:hidden">
				<Sheet.Header>
					<Sheet.Title>
						<img src="{assets}/immagini/lightblue-logo.svg" alt="Logo" class="h-9" />
					</Sheet.Title>
					<div class="space-y-2 p-4">
						{#each links as link}
							<MobileMenuLink url={link.url} testo={link.testo} />
						{/each}
					</div>
				</Sheet.Header>
			</Sheet.Content>
		</Sheet.Root>
	</nav>
</div>
