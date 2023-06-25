<script lang="ts">
	import ButtonFreeQuotation from '$lib/components/ButtonFreeQuotation.svelte';
	import { AppBar, LightSwitch, drawerStore } from '@skeletonlabs/skeleton';
	import NavigationLinks from './NavigationLinks.svelte';
	import IoIosMenu from 'svelte-icons/io/IoIosMenu.svelte';
	import type { DrawerSettings } from '@skeletonlabs/skeleton';

	const settingsDrawerMenuMobile: DrawerSettings = {
		id: 'menu-mobile',
		bgDrawer: 'bg-primary-50-900-token',
		bgBackdrop: '',
		width: 'w-full',
		padding: 'pl-8 pt-8 pb-8',
		rounded: 'rounded-l-3xl',
		position: 'right'
	};

	const handleClickOpenMenuMobile = () => {
		drawerStore.open(settingsDrawerMenuMobile);
	};
</script>

<AppBar background="bg-surface-50-900-token " padding="py-2 px-4" spacing="space-y-0" gap="'gap-0">
	<svelte:fragment slot="lead">
		<img
			src="images/logo.png"
			class="min-w-20 aspect-square w-20 min-w-[50px] cursor-pointer"
			alt="logo de la patisserie féérie sucrée"
		/>
	</svelte:fragment>
	<svelte:fragment slot="trail">
		<NavigationLinks />
		<div class="hidden h-6 w-12 lg:block">
			<LightSwitch />
		</div>
		<ButtonFreeQuotation />
		<button on:click={handleClickOpenMenuMobile} type="button" class="btn-icon block lg:hidden"
			><IoIosMenu class="" /></button
		>
	</svelte:fragment>
</AppBar>
