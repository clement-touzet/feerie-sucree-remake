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

<a
	href="/severine-touzet"
	on:click={handleCloseDrawer}
	class="btn text-2xl font-medium text-primary-500 dark:text-primary-50 block"
>
	Séverine touzet
</a>

<a
	on:click={handleCloseDrawer}
	href="/mes-creations"
	class="btn text-2xl font-medium text-primary-500 dark:text-primary-50 block"
>
	Mes créations
</a>

<a
	on:click={handleCloseDrawer}
	href="/blog"
	class="btn text-2xl font-medium text-primary-500 dark:text-primary-50 block"
>
	Blog
</a>
<a
	on:click={handleCloseDrawer}
	href="/info-et-contact"
	class="btn text-2xl font-medium text-primary-500 dark:text-primary-50 block"
>
	Contact
</a>
