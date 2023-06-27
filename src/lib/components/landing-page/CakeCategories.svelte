<script>
	import { mesCreationsRoute } from '$lib/utils/constants/routes';
	import CakeCategorieCard from '../cakes/categories/CakeCategorieCard.svelte';
</script>

<div class="paddingAndMarginContainer text-center">
	<h2 class="h2">Choisissez votre type de gâteaux</h2>
	<div class="no-scrollbar mx-auto mt-4 flex max-w-screen-xl gap-8 overflow-y-auto px-4">
		<CakeCategorieCard />
		<CakeCategorieCard />
		<CakeCategorieCard />
		<CakeCategorieCard />
	</div>
	<a
		class="md:btn-lg btn-md btn mt-8 w-auto cursor-pointer bg-gradient-to-r from-secondary-500 to-primary-500 font-medium text-white md:w-96"
		href={mesCreationsRoute}
	>
		Voir toutes les catégories
	</a>
</div>
