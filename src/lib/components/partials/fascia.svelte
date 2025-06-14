<script lang="ts">
	export let titolo: string;
	export let desc: string;
</script>

<div class="bg-primary flex w-full flex-col items-center justify-center gap-2 p-2">
	<h1 class="text-4xl font-bold text-white">{titolo}</h1>
	<p class="italic">{desc}</p>
</div>
