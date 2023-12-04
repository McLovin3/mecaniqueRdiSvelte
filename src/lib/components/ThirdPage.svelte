<script lang="ts">
	import { _ } from "svelte-i18n";
	import { Splide, SplideSlide } from "@splidejs/svelte-splide";
	import "@splidejs/svelte-splide/css";
</script>

<section class="h-screen flex flex-col justify-center">
	<div
		class="h-2/3 bg-surface-600 rounded-xl w-2/3 mx-auto flex flex-col justify-center text-white"
	>
		<Splide
			options={{
				autoplay: true,
				pauseOnFocus: true,
				rewind: true
			}}
			class="h-full flex flex-col justify-center"
		>
			<SplideSlide>
				<div class="flex flex-row justify-center w-2/3 mx-auto">
					<h1 class="text-4xl font-bold text-center">
						Lorem ipsum dolor sit amet, consectetur adipisicing elit. A impedit omnis commodi, non,
						aspernatur similique amet soluta necessitatibus voluptatem expedita quam iste dolore
						reiciendis dignissimos unde saepe id! Odio, possimus.
					</h1>
					<img src="placeholder.jpg" alt="placeholder" />
				</div>
			</SplideSlide>
			<SplideSlide>
				<div class="flex flex-row justify-center w-2/3 mx-auto">
					<h1 class="text-4xl font-bold text-center">
						Lorem ipsum dolor sit amet, consectetur adipisicing elit. A impedit omnis commodi, non,
						aspernatur similique amet soluta necessitatibus voluptatem expedita quam iste dolore
						reiciendis dignissimos unde saepe id! Odio, possimus.
					</h1>
					<img src="placeholder.jpg" alt="placeholder" />
				</div>
			</SplideSlide>
			<SplideSlide>
				<div class="flex flex-row justify-center w-2/3 mx-auto">
					<h1 class="text-4xl font-bold text-center">
						Lorem ipsum dolor sit amet, consectetur adipisicing elit. A impedit omnis commodi, non,
						aspernatur similique amet soluta necessitatibus voluptatem expedita quam iste dolore
						reiciendis dignissimos unde saepe id! Odio, possimus.
					</h1>
					<img src="placeholder.jpg" alt="placeholder" />
				</div>
			</SplideSlide>
			<SplideSlide>
				<div class="flex flex-row justify-center w-2/3 mx-auto">
					<h1 class="text-4xl font-bold text-center">
						Lorem ipsum dolor sit amet, consectetur adipisicing elit. A impedit omnis commodi, non,
						aspernatur similique amet soluta necessitatibus voluptatem expedita quam iste dolore
						reiciendis dignissimos unde saepe id! Odio, possimus.
					</h1>
					<img src="placeholder.jpg" alt="placeholder" />
				</div>
			</SplideSlide>
		</Splide>
	</div>
</section>
