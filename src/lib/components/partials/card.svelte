<script lang="ts">
	import { assets } from '$app/paths';
	import type { Progetto } from './progetti';

	let p: Progetto = $props();
</script>

<div>
	<img src="{assets}/immagini/progetti/{p.immagine}" alt="Immagine di {p.titolo}" />
	<div>
		<p>{p.immagine}</p>
		<p>{p.titolo}</p>
	</div>
</div>
