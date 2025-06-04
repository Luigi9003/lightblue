<script lang="ts">
	import { base } from '$app/paths';

	type Attributi = {
		url: string;
		testo: string;
	};

	let a: Attributi = $props();
</script>

<a href="{base}{a.url}" class="text-primary-foreground hover:text-primary block">{a.testo}</a>
