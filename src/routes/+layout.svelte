<script lang="ts">
	// The ordering of these imports is critical to your app working properly
	import '@skeletonlabs/skeleton/themes/theme-skeleton.css';
	// If you have source.organizeImports set to true in VSCode, then it will auto change this ordering
	import '@skeletonlabs/skeleton/styles/skeleton.css';
	// Most of your app wide CSS should be put in this file
	import '../app.postcss';
	import { AppShell, Drawer, drawerStore } from '@skeletonlabs/skeleton';
	import Navbar from '$lib/layouts/navbar/Navbar.svelte';
	import MenuMobileDrawerContent from '$lib/layouts/navbar/mobile/MenuMobileDrawerContent.svelte';
</script>

<Drawer slotContent="bg-surface-50-900-token">
	{#if $drawerStore.id === 'menu-mobile'}
		<MenuMobileDrawerContent />
	{/if}
</Drawer>

<AppShell slotPageContent="bg-surface-50-900-token ">
	<svelte:fragment slot="header">
		<Navbar />
	</svelte:fragment>
	<slot />
</AppShell>
