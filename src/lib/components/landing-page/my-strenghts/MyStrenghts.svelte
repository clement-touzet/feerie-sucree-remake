<script>
	import ArtisanatStrenght from './ArtisanatStrenght.svelte';
	import EcoFriendlyStrenght from './EcoFriendlyStrenght.svelte';
	import PassionStrength from './PassionStrength.svelte';
</script>

<div class="paddingAndMarginContainer mx-auto max-w-screen-xl items-center text-center">
	<h2 class="h2 text-5xl font-black">Mes forces</h2>
	<div class=" mt-4 flex flex-col gap-16">
		<ArtisanatStrenght />
		<EcoFriendlyStrenght />
		<PassionStrength />
	</div>
</div>
