<script>
	import { drawerStore } from '@skeletonlabs/skeleton';

	const handleCloseDrawer = () => {
		drawerStore.close();
	};
</script>

<a
	href="/"
	on:click={handleCloseDrawer}
	class="btn text-2xl font-medium text-primary-500 dark:text-primary-50 block"
>
	Accueil
</a>

<a href="/cake-design" class="btn text-2xl font-medium text-primary-500 dark:text-primary-50 block">
	Mes réalisations
</a>

<a href="/accueil" class="btn text-2xl font-medium text-primary-500 dark:text-primary-50 block">
	Blog
</a>
