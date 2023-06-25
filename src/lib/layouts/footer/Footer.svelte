<script>
	import {
		accueilRoute,
		blogRoute,
		infoAndContactRoute,
		mesCreationsRoute,
		severineTouzetRoute
	} from '$lib/utils/constants/routes';
</script>

<div
	class="mt-8 flex flex-wrap items-center gap-16 bg-surface-900 p-8 text-white dark:bg-surface-800 md:mt-16 md:flex-row md:justify-center"
>
	<div class="">
		<img
			src="images/logo.png"
			class="min-w-20 aspect-square w-20 min-w-[50px] cursor-pointer"
			alt="logo de la patisserie féérie sucrée"
		/>
	</div>
	<div class="flex flex-col gap-2">
		<a href={accueilRoute}>Accueil</a>
		<a href={blogRoute}>Blog</a>
		<a href={infoAndContactRoute}>Contact</a>
		<a href={mesCreationsRoute}>Mes créations</a>
		<a href={severineTouzetRoute}>Severine Touzet</a>
	</div>
	<div class="flex flex-col gap-2">
		<a href={''}>Mentions légales</a>
		<a href={''}>TODO</a>
		<a href={''}>Politique de confidentialité</a>
	</div>
</div>
