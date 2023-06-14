<script lang="ts">
	import { LightSwitch, drawerStore } from '@skeletonlabs/skeleton';
	import MdClose from 'svelte-icons/md/MdClose.svelte';
	import MobileNavigationLinks from './MobileNavigationLinks.svelte';

	const handleClickCloseDrawer = () => {
		drawerStore.close();
	};
</script>

<div class="flex h-full w-full flex-col items-center overflow-auto p-4">
	<div class="flex w-full flex-row-reverse">
		<button class="btn-icon" on:click={handleClickCloseDrawer}><MdClose /></button>
	</div>
	<div class="item-center my-4 flex h-full w-full flex-col justify-center gap-4">
		<MobileNavigationLinks />
	</div>

	<LightSwitch />
</div>
