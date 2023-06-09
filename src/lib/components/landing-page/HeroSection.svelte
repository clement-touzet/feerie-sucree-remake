<script>
	import ButtonFreeQuotation from '../ButtonFreeQuotation.svelte';
</script>

<section class="">
	<div class="grid max-w-screen-xl px-4 py-8 mx-auto lg:gap-8 xl:gap-0 lg:py-16 lg:grid-cols-12">
		<div class="mr-auto place-self-center lg:col-span-7">
			<h1
				class="h1 max-w-2xl mb-4 text-4xl font-extrabold tracking-tight leading-none md:text-5xl xl:text-6xl"
			>
				Les
				<span
					class="bg-gradient-to-br from-secondary-500 to-primary-500 to-70% bg-clip-text text-transparent box-decoration-clone"
				>
					meilleurs
				</span> gâteaux de la région
			</h1>
			<p
				class="max-w-2xl mb-6 font-normal text-gray-400 lg:mb-8 md:text-lg lg:text-xl dark:text-gray-400"
			>
				Je réalise le gateau de vos rêves, que ce soit pour un mariage, une baby shower, un
				anniversaire, et bien plus encore... Toutes mes patisseries sont faites entièrement à la
				main.
			</p>
			<ButtonFreeQuotation />
		</div>
		<div class="hidden lg:mt-0 lg:col-span-5 lg:flex">
			<img
				class="rounded-3xl shadow-lg max-w-md object-cover"
				src="images/patisseries/bandeau-licorne-accueil.jpg"
				alt="licorne en pâte à sucre"
			/>
		</div>
	</div>
</section>
