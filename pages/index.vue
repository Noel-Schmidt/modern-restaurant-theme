<template>
	<div id="navigation" class="absolute top-0 left-0 w-full">
		<div class="max-w-[105rem] mx-auto py-8 px-5">
			<div class="flex justify-between">
				<div class="">
					<p class="font-['Hurme-Black'] text-2xl -mb-1 p-0">Foody</p>
					<p class="font-['Hurme-Light']">Restaurant & Bar</p>
				</div>

				<button class="bg-black flex w-14 h-14 items-center justify-center rounded-xl rounded-br-3xl">
					<ShoppingCartIcon class="inline h-8 w-8 text-white" aria-hidden="true" />
				</button>
			</div>

		</div>
	</div>

	<div class="max-w-[105rem] mx-auto py-8 px-5">
		<div id="hero">
			<div class="grid grid-cols-5 flex justify-space items-center">
				<div class="col-span-5 md:col-span-2 mt-24 md:mt-0">
					<div class="font-['Hurme-Black'] text-7xl">
						Delicious<br/>Food for you<br/>At home!
					</div>

					<div class="mt-24">
						<NuxtLink to="#" class="bg-black text-white px-6 py-5 text-2xl font-['Hurme-Semi'] shadow-2xl rounded-3xl rounded-br-none">
							View Menu
							<ArrowNarrowRightIcon class="inline mb-2 h-6 w-6 text-white ml-8" aria-hidden="true" />
						</NuxtLink>
					</div>

					<div class="mt-24 flex gap-4">
						<NuxtLink class="bg-white flex w-20 w-20 items-center justify-center drop-shadow-2xl rounded-2xl p-6" to="#">
							<img class="min-w-[2.4rem]" src="/images/icons/burger.svg" alt="Burger">
						</NuxtLink>

						<NuxtLink class="bg-white flex w-20 w-20 items-center justify-center drop-shadow-2xl rounded-2xl p-6" to="#">
							<img class="min-w-[2.4rem]" src="/images/icons/cold-drink.svg" alt="Drinks">
						</NuxtLink>

						<NuxtLink class="bg-white flex w-20 w-20 items-center justify-center drop-shadow-2xl rounded-2xl p-6" to="#">
							<img class="min-w-[2.4rem]" src="/images/icons/hot-soup.svg" alt="Soups">
						</NuxtLink>

						<NuxtLink class="bg-white flex w-20 w-20 items-center justify-center drop-shadow-2xl rounded-2xl p-6" to="#">
							<img class="min-w-[2.4rem]" src="/images/icons/popsicle.svg" alt="Ice">
						</NuxtLink>
					</div>
				</div>

				<div class="hidden md:block col-span-3">
					<img class="max-w-4xl" alt="Stock Image" src="/images/stock-image-01.webp">
				</div>
			</div>
		</div>

		<div id="products" class="mt-40 md:mt-12">
			<div class="grid grid-cols-2 lg:grid-cols-10 gap-10">
				<div class="col-span-8 lg:col-span-2 bg-white rounded-3xl shadow-2xl">
					<div class="flex justify-center">
						<img class="max-w-screen-[17rem] -mt-24" alt="Stock Image" src="/images/stock-image-01.webp">
					</div>

					<div class="px-8 p-6">
						<div class="text-2xl font-['Hurme-Bold']">
							Curry Bowl
						</div>

						<div class="text-sm -mt-1">
							Spicy Curry with chicken
						</div>

						<div class="font-['Hurme-Bold'] mt-3 -mb-5">
							$ 22,50
						</div>
					</div>

					<div class="flex justify-end -mb-7 mr-5">
						<button class="bg-black flex w-14 h-14 items-center justify-center rounded-xl rounded-br-3xl">
							<ShoppingCartIcon class="inline h-8 w-8 text-white" aria-hidden="true" />
						</button>
					</div>
				</div>

				<div class="col-span-8 mt-24 lg:mt-0 lg:col-span-2 bg-white rounded-3xl shadow-2xl">
					<div class="flex justify-center">
						<img class="max-w-screen-[17rem] -mt-24" alt="Stock Image" src="/images/stock-image-02.webp">
					</div>

					<div class="px-8 p-6">
						<div class="text-2xl font-['Hurme-Bold']">
							Salad Bowl
						</div>

						<div class="text-sm -mt-1">
							Hot Salad with chicken
						</div>

						<div class="font-['Hurme-Bold'] mt-3 -mb-5">
							$ 12,50
						</div>
					</div>

					<div class="flex justify-end -mb-7 mr-5">
						<button class="bg-black flex w-14 h-14 items-center justify-center rounded-xl rounded-br-3xl">
							<ShoppingCartIcon class="inline h-8 w-8 text-white" aria-hidden="true" />
						</button>
					</div>
				</div>


				<div class="col-span-6 items-center ml-0 md:ml-32">
					<div class="flex">
						<div class="text-6xl font-['Hurme-Bold'] max-w-xl">Delicious selection of countless dishes</div>
					</div>

					<div class="mt-6 max-w-xl font-['Hurme-SemiBold']">
						Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed diam nonumy eirmod tempor invidunt ut labore
						et dolore magna aliquyam erat, sed diam voluptua. 	Lorem ipsum dolor sit amet, consetetur sadipscing elitr, sed
					</div>
				</div>

			</div>


		</div>

	</div>
</template>

<script>
import {
	ArrowNarrowRightIcon,
	ShoppingCartIcon
} from '@heroicons/vue/outline'

export default {
	components: {
		ArrowNarrowRightIcon,
		ShoppingCartIcon
	},

	setup() {
		useHead({
			htmlAttrs: {
				class: "bg-slate-100 overflow-x-hidden"
			}
		})
	}
}
</script>
