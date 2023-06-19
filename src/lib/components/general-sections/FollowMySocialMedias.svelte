<script>
	import FacebookLogo from '$lib/svg/FacebookLogo.svelte';
	import InstagramLogo from '$lib/svg/InstagramLogo.svelte';
	import { facebookLink, instagramLink } from '$lib/utils/constants/socialLinks';
</script>

<div class="mt-8 flex flex-col items-center gap-6 p-6 text-center bg-primary-50-900-token md:mt-16">
	<p class="text-xl font-medium">
		Rejoingnez-moi sur les réseaux sociaux pour voir toutes mes créations !
	</p>
	<div class="flex gap-6">
		<a href={instagramLink} target="_blank">
			<InstagramLogo height={36} width={36} />
		</a>
		<a href={facebookLink} target="_blank">
			<FacebookLogo height={36} width={36} />
		</a>
	</div>
</div>
