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
		'block',
		{ 'text-primary': isActive, 'text-primary-foreground hover:text-primary': !isActive }
	]}
>
	{a.testo}
</a>
