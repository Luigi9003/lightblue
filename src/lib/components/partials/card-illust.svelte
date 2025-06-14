<script lang="ts">
	import { assets } from '$app/paths';
	export let titolo: string;
	export let immagine: string;
	export let desc: string;
</script>

<div class="max-w-sm bg-white">
	<img
		class="h-sm flex w-sm justify-items-center"
		src="{assets}/immagini/illustrazioni/{immagine}"
		alt={titolo}
	/>
	<div class="bg-primary p-2">
		<h2 class="text-xl font-bold text-white">{titolo}</h2>
	</div>
	<div class="bg-primary p-2 pt-0 italic">
		{desc}
	</div>
</div>
