<script lang="ts">
	import { base } from '$app/paths';
	import { page } from '$app/state';

	type Attributo = {
		url: string;
		testo: string;
	};

	let a: Attributo = $props();

	const href = $derived(base + a.url);
	const isActive = $derived(page.url.pathname == href);
</script>

<a
	{href}
	class={[
		'block p-2',
		'rounded-md text-center',
		{
			'text-secondary-foreground hover:text-primary hover:bg-primary/10': !isActive,
			'bg-primary text-secondary': isActive
		}
	]}
>
	{a.testo}
</a>
