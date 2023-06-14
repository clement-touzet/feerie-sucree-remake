<script lang="ts">
	import EmailIcon from '$lib/svg/EmailIcon.svelte';
	import FacebookLogo from '$lib/svg/FacebookLogo.svelte';
	import LocationIcon from '$lib/svg/LocationIcon.svelte';
	import InstagramLogo from '../../svg/InstagramLogo.svelte';
	import InterractiveMap from './InterractiveMap.svelte';
</script>

<div
	class="px:4 mx-auto mt-8 flex max-w-screen-lg flex-col items-center gap-20 md:px-8 lg:flex-row"
>
	<!-- contact links card -->
	<div
		class="card grid flex-1 grid-cols-[32px_auto] content-center items-center justify-center gap-8 p-8 bg-primary-50-900-token"
	>
		<div>
			<InstagramLogo height={32} width={32} />
		</div>
		<p class="text-lg">severinetouzet</p>
		<div class="">
			<FacebookLogo height={32} width={32} />
		</div>
		<p class="text-lg">feeriesucreetarnos</p>
		<div class="">
			<EmailIcon height={32} width={32} />
		</div>
		<p class="text-lg">sedes52@gmail.com</p>
		<div class="">
			<LocationIcon height={32} width={32} />
		</div>
		<div>
			<p class="text-lg">39 Rue Lucien Barbier</p>
			<p class="text-lg">40220, Tarnos</p>
		</div>
	</div>
	<!-- map card -->
	<div class="flex-1">
		<InterractiveMap />
	</div>
</div>
