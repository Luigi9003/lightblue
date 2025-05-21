<script lang="ts">
	type Attributi = {
		url: string;
		testo: string;
	};

	let a: Attributi = $props();
</script>

<a href={a.url} class="text-primary-foreground hover:text-primary block">{a.testo}</a>
