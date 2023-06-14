<script>
	import ButtonFreeQuotation from '../ButtonFreeQuotation.svelte';
</script>

<section class="">
	<div class="mx-auto grid max-w-screen-xl px-4 py-8 lg:grid-cols-12 lg:gap-8 lg:py-16 xl:gap-0">
		<div class="mr-auto place-self-center lg:col-span-7">
			<h1
				class="h1 mb-4 max-w-2xl text-4xl font-extrabold leading-none tracking-tight md:text-5xl xl:text-6xl"
			>
				Les
				<span
					class="bg-gradient-to-br from-secondary-500 to-primary-500 to-70% box-decoration-clone bg-clip-text text-transparent"
				>
					meilleurs
				</span> gâteaux de la région
			</h1>
			<p
				class="mb-6 max-w-2xl font-normal text-gray-400 dark:text-gray-400 md:text-lg lg:mb-8 lg:text-xl"
			>
				Je réalise le gateau de vos rêves, que ce soit pour un mariage, une baby shower, un
				anniversaire, et bien plus encore... Toutes mes patisseries sont faites entièrement à la
				main.
			</p>
			<ButtonFreeQuotation />
		</div>
		<div class="hidden lg:col-span-5 lg:mt-0 lg:flex">
			<img
				class="max-w-md rounded-3xl object-cover shadow-lg"
				src="images/patisseries/bandeau-licorne-accueil.jpg"
				alt="licorne en pâte à sucre"
			/>
		</div>
	</div>
</section>
