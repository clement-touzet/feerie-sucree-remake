<script>
	import CardAllContactLinks from '$lib/components/info-et-contact/CardAllContactLinks.svelte';
	import ContactHeroSection from '$lib/components/info-et-contact/ContactHeroSection.svelte';
	import FirstParagraph from '$lib/components/info-et-contact/FirstParagraph.svelte';
	import ParagraphOnPlace from '$lib/components/info-et-contact/ParagraphOnPlace.svelte';
</script>

<svelte:head>
	<title>Féérie Sucrée - Contact</title>
</svelte:head>

<div class="mb-16">
	<ContactHeroSection />
	<FirstParagraph />
	<CardAllContactLinks />

	<ParagraphOnPlace />
</div>
