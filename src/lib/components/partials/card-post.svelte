<script lang="ts">
	import { assets } from '$app/paths';
	export let titolo: string;
	export let immagine: string;
</script>

<div class="bg-secondary max-w-sm overflow-hidden p-2">
	<img
		class="h-sm flex w-sm justify-items-center"
		src="{assets}/immagini/progetti/{immagine}"
		alt={titolo}
	/>
	<div class="pt-2 pb-2">
		<h2 class="text-primary text-xl font-bold">{titolo}</h2>
	</div>
</div>
