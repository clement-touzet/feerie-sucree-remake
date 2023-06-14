<script>
	import { drawerStore } from '@skeletonlabs/skeleton';

	const handleCloseDrawer = () => {
		drawerStore.close();
	};
</script>

<a
	href="/"
	on:click={handleCloseDrawer}
	class="btn block text-2xl font-medium text-primary-500 dark:text-primary-50"
>
	Accueil
</a>

<a
	href="/severine-touzet"
	on:click={handleCloseDrawer}
	class="btn block text-2xl font-medium text-primary-500 dark:text-primary-50"
>
	Séverine touzet
</a>

<a
	on:click={handleCloseDrawer}
	href="/mes-creations"
	class="btn block text-2xl font-medium text-primary-500 dark:text-primary-50"
>
	Mes créations
</a>

<a
	on:click={handleCloseDrawer}
	href="/blog"
	class="btn block text-2xl font-medium text-primary-500 dark:text-primary-50"
>
	Blog
</a>
<a
	on:click={handleCloseDrawer}
	href="/info-et-contact"
	class="btn block text-2xl font-medium text-primary-500 dark:text-primary-50"
>
	Contact
</a>
