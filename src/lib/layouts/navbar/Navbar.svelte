<script lang="ts">
	import ButtonFreeQuotation from '$lib/components/ButtonFreeQuotation.svelte';
	import { AppBar, LightSwitch, drawerStore } from '@skeletonlabs/skeleton';
	import NavigationLinks from './NavigationLinks.svelte';
	import IoIosMenu from 'svelte-icons/io/IoIosMenu.svelte';
	import type { DrawerSettings } from '@skeletonlabs/skeleton';

	const settingsDrawerMenuMobile: DrawerSettings = {
		id: 'menu-mobile',
		bgDrawer: 'bg-primary-50-900-token',
		bgBackdrop:
			'bg-gradient-to-br from-primary-500/50 to-secondary-500/50 dark:from-primary-500/80 dark:to-secondary-500/80',
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
		<!-- todo button menu drawer -->
		<img
			src="images/logo.png"
			class="w-20 aspect-square min-w-20 cursor-pointer min-w-[50px]"
			alt="logo de la patisserie féérie sucrée"
		/>
	</svelte:fragment>
	<svelte:fragment slot="trail">
		<NavigationLinks />
		<div class="w-12 h-6 hidden lg:block">
			<LightSwitch />
		</div>
		<ButtonFreeQuotation />
		<button on:click={handleClickOpenMenuMobile} type="button" class="btn-icon block lg:hidden"
			><IoIosMenu class="" /></button
		>
	</svelte:fragment>
</AppBar>
