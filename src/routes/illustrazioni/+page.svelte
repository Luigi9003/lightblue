<script>
	import Card from '$lib/components/partials/card-illust.svelte';
	import Fascia from '$lib/components/partials/fascia.svelte';
</script>

<div class="flex w-full flex-col">
	<Fascia
		titolo="Illustrazioni per la stampa"
		desc="Disegni digitali realizzati per essere stampati, con attenzione a colori e composizione"
	/>

	<div
		class="mx-auto grid w-full place-items-center items-start gap-4 p-4 sm:grid-cols-1 md:grid-cols-2 xl:grid-cols-3"
	>
		<Card
			titolo="Intio di compleanno"
			immagine="invito-compleanno.jpg"
			desc="Invito di compleanno con grafica personalizzata e illustrazione su richiesta"
		/>
		<Card
			titolo="Quadro di famiglia"
			immagine="quadro-family.jpg"
			desc="Ritratto illustrato digitalmente e successivamente stampato su tela"
		/>
	</div>

	<Fascia
		titolo="Creatività per i social"
		desc="Un mix di ritratti e illustrazioni, tra sperimentazione e stile personale"
	/>

	<div
		class="mx-auto grid w-full place-items-center items-start gap-4 p-4 sm:grid-cols-1 md:grid-cols-2 xl:grid-cols-3"
	>
		<Card
			titolo="Lana Parrilla"
			immagine="lana-parrilla.jpg"
			desc="Ritratto dell'attrice ispirato al personaggio 'Regina' nella serie 'Once Upon a Time'"
		/>
		<Card
			titolo="Lorenzo Branchetti"
			immagine="lorenzo-branchetti-milo-cotogno.jpg"
			desc="Ritratto ispirato al personaggio 'Milo Cotogno' della Melevisione "
		/>
		<Card titolo="Pin Up" immagine="pin-up.jpg" desc="Illustrazione ispirata agli anni 50" />
		<Card
			titolo="Katy Pery"
			immagine="katy-perry.jpg"
			desc="Ritratto della cantautrice statunitense"
		/>
		<Card
			titolo="Marinaio"
			immagine="marinaio.jpg"
			desc="Illustrazione nata per unire il mare e il lounge bar"
		/>
		<Card
			titolo="Mantieni il bacio"
			immagine="mantieni-il-bacio.jpg"
			desc="Illustrazione nata dall'ispirazione della canzone di Michele Bravi"
		/>
		<Card
			titolo="Lorella Boccia"
			immagine="lorella-boccia.jpg"
			desc="Ritratto della ballerina e conduttrice televisiva italiana"
		/>
		<Card
			titolo="Made in Italy"
			immagine="made-in-italy.jpg"
			desc="Illustrazione ispirata dalla canzone di Rosa Chemical"
		/>
		<Card
			titolo="My muse"
			immagine="vale.jpg"
			desc="Ritratto per una delle persone che ha sempre creduto in me"
		/>
	</div>
</div>
