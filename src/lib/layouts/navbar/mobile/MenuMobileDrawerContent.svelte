<script lang="ts">
	import { LightSwitch, drawerStore } from '@skeletonlabs/skeleton';
	import MdClose from 'svelte-icons/md/MdClose.svelte';
	import MobileNavigationLinks from './MobileNavigationLinks.svelte';

	const handleClickCloseDrawer = () => {
		drawerStore.close();
	};
</script>

<div class="flex flex-col items-center h-full w-full p-4 overflow-auto">
	<div class="flex flex-row-reverse w-full">
		<button class="btn-icon" on:click={handleClickCloseDrawer}><MdClose /></button>
	</div>
	<div class="flex flex-col gap-4 item-center justify-center w-full h-full my-4">
		<MobileNavigationLinks />
	</div>

	<LightSwitch />
</div>
