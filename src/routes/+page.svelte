<script>
	// @ts-nocheck
	import Carousel from '$lib/carousel.svelte';

	let x;
	let y;

	const images = [
		'https://images.pexels.com/photos/1001682/pexels-photo-1001682.jpeg?auto=compress&cs=tinysrgb&w=600',
		'https://images.pexels.com/photos/1001682/pexels-photo-1001682.jpeg?auto=compress&cs=tinysrgb&w=600',
		'https://images.pexels.com/photos/1001682/pexels-photo-1001682.jpeg?auto=compress&cs=tinysrgb&w=600',
		'https://images.pexels.com/photos/1001682/pexels-photo-1001682.jpeg?auto=compress&cs=tinysrgb&w=600'
	];
</script>

<svelte:window bind:innerHeight={y} bind:innerWidth={x} />
<!-- hero -->
<div class="hero min-h-screen" style="background-image: url(tzu_shao_hero.jpg);">
	<div class="hero-overlay bg-opacity-60"></div>
	<div class="hero-content text-center text-neutral-content">
		<div class="max-w-md">
			<h1 class="mb-5 text-5xl font-bold">Tzu Shao Northeast Region</h1>
			<p class="mb-5">
				Tzu Chi Youth Group, also known as “Tzu Shao.” Young volunteers learn to care with Tzu Chi’s
				love and humanistic spirit.
			</p>
			<a href="https://forms.gle/bu7B421sdPcShbqX6" target="_blank" rel="noopener noreferrer">
				<button class="btn btn-primary">Sign Up</button>
			</a>
		</div>
	</div>
</div>
<!-- carousel -->
<div class="flex flex-col items-center justify-center">
	<h2
		class="max-w-lg m-10 text-3xl font-semibold leading-normal text-gray-900 dark:text-white text-center"
	>
		Our Activities
	</h2>
	<div class="carousel w-full">
		<div id="slide1" class="carousel-item relative w-full">
			<img src="src/lib/ocean.jpg" class="w-full" />
			<div class="absolute flex justify-between transform -translate-y-1/2 left-5 right-5 top-1/2">
				<a href="#slide4" class="btn btn-circle">❮</a>
				<a href="#slide2" class="btn btn-circle">❯</a>
			</div>
		</div>
		<div id="slide2" class="carousel-item relative w-full">
			<img src="src/lib/ocean.jpg" class="w-full" />
			<div class="absolute flex justify-between transform -translate-y-1/2 left-5 right-5 top-1/2">
				<a href="#slide1" class="btn btn-circle">❮</a>
				<a href="#slide3" class="btn btn-circle">❯</a>
			</div>
		</div>
		<div id="slide3" class="carousel-item relative w-full">
			<img src="src/lib/ocean.jpg" class="w-full" />
			<div class="absolute flex justify-between transform -translate-y-1/2 left-5 right-5 top-1/2">
				<a href="#slide2" class="btn btn-circle">❮</a>
				<a href="#slide4" class="btn btn-circle">❯</a>
			</div>
		</div>
		<div id="slide4" class="carousel-item relative w-full">
			<img src="src/lib/ocean.jpg" class="w-full" />
			<div class="absolute flex justify-between transform -translate-y-1/2 left-5 right-5 top-1/2">
				<a href="#slide3" class="btn btn-circle">❮</a>
				<a href="#slide1" class="btn btn-circle">❯</a>
			</div>
		</div>
	</div>
</div>

<!-- body -->
<div class="flex flex-col items-center justify-center">
	<h2
		class="max-w-lg m-10 text-3xl font-semibold leading-normal text-gray-900 dark:text-white text-center"
	>
		Our Core Values
	</h2>
	{#if x > y}
		<div class="flex w-full">
			<div class="card w-96 bg-base-100 shadow-xl">
				<figure>
					<img src="src/lib/ocean.jpg" alt="Shoes" />
				</figure>
				<div class="card-body">
					<h2 class="card-title">Shoes!</h2>
					<p>If a dog chews shoes whose shoes does he choose?</p>
					<div class="card-actions justify-end">
						<button class="btn btn-primary">Buy Now</button>
					</div>
				</div>
			</div>
			<div class="divider divider-horizontal"></div>
			<div class="card w-96 bg-base-100 shadow-xl">
				<figure>
					<img src="src/lib/ocean.jpg" alt="Shoes" />
				</figure>
				<div class="card-body">
					<h2 class="card-title">Shoes!</h2>
					<p>If a dog chews shoes whose shoes does he choose?</p>
					<div class="card-actions justify-end">
						<button class="btn btn-primary">Buy Now</button>
					</div>
				</div>
			</div>
			<div class="divider divider-horizontal"></div>
			<div class="card w-96 bg-base-100 shadow-xl">
				<figure>
					<img src="src/lib/ocean.jpg" alt="Shoes" />
				</figure>
				<div class="card-body">
					<h2 class="card-title">Shoes!</h2>
					<p>If a dog chews shoes whose shoes does he choose?</p>
					<div class="card-actions justify-end">
						<button class="btn btn-primary">Buy Now</button>
					</div>
				</div>
			</div>
			<div class="divider divider-horizontal"></div>
			<div class="card w-96 bg-base-100 shadow-xl">
				<figure>
					<img src="src/lib/ocean.jpg" alt="Shoes" />
				</figure>
				<div class="card-body">
					<h2 class="card-title">Shoes!</h2>
					<p>If a dog chews shoes whose shoes does he choose?</p>
					<div class="card-actions justify-end">
						<button class="btn btn-primary">Buy Now</button>
					</div>
				</div>
			</div>
		</div>
	{:else}
		<div class="grid grid-cols-2 gap-4">
			<div class="card w-48 bg-base-100 shadow-xl">
				<figure>
					<img src="src/lib/ocean.jpg" alt="Shoes" />
				</figure>
				<div class="card-body">
					<h2 class="card-title">Medicine</h2>
					<p>If a dog chews shoes whose shoes does he choose?</p>
					<div class="card-actions justify-end">
						<button class="btn btn-primary">Learn More</button>
					</div>
				</div>
			</div>
			<div class="card w-48 bg-base-100 shadow-xl">
				<figure>
					<img src="src/lib/ocean.jpg" alt="Shoes" />
				</figure>
				<div class="card-body">
					<h2 class="card-title">Charity</h2>
					<p>If a dog chews shoes whose shoes does he choose?</p>
					<div class="card-actions justify-end">
						<button class="btn btn-primary">Learn More</button>
					</div>
				</div>
			</div>
			<div class="card w-48 bg-base-100 shadow-xl">
				<figure>
					<img src="src/lib/ocean.jpg" alt="Shoes" />
				</figure>
				<div class="card-body">
					<h2 class="card-title">Culture</h2>
					<p>If a dog chews shoes whose shoes does he choose?</p>
					<div class="card-actions justify-end">
						<button class="btn btn-primary">Learn More</button>
					</div>
				</div>
			</div>
			<div class="card w-48 bg-base-100 shadow-xl">
				<figure>
					<img src="src/lib/ocean.jpg" alt="Shoes" />
				</figure>
				<div class="card-body">
					<h2 class="card-title">Education</h2>
					<p>If a dog chews shoes whose shoes does he choose?</p>
					<div class="card-actions justify-end">
						<button class="btn btn-primary">Learn More</button>
					</div>
				</div>
			</div>
		</div>
	{/if}
</div>

<div class="flex flex-col items-center justify-center">
	<h2
		class="max-w-lg m-10 text-3xl font-semibold leading-normal text-gray-900 dark:text-white text-center"
	>
		Coordinator
	</h2>
	<div class="avatar">
		<div class="w-24 rounded">
			<img src="src/lib/ocean.jpg" />
		</div>
	</div>
	<p class="text-lg font-medium text-gray-900 dark:text-white">Name</p>
	<p class="text-md font-medium text-gray-900 dark:text-white">My favorite hobby is</p>
	<p class="text-md font-medium text-gray-900 dark:text-white">Email:</p>
	<br />
</div>

<footer class="footer p-10 bg-neutral text-neutral-content">
	<aside>
		<svg
			width="50"
			height="50"
			viewBox="0 0 24 24"
			xmlns="http://www.w3.org/2000/svg"
			fill-rule="evenodd"
			clip-rule="evenodd"
			class="fill-current"
			><path
				d="M22.672 15.226l-2.432.811.841 2.515c.33 1.019-.209 2.127-1.23 2.456-1.15.325-2.148-.321-2.463-1.226l-.84-2.518-5.013 1.677.84 2.517c.391 1.203-.434 2.542-1.831 2.542-.88 0-1.601-.564-1.86-1.314l-.842-2.516-2.431.809c-1.135.328-2.145-.317-2.463-1.229-.329-1.018.211-2.127 1.231-2.456l2.432-.809-1.621-4.823-2.432.808c-1.355.384-2.558-.59-2.558-1.839 0-.817.509-1.582 1.327-1.846l2.433-.809-.842-2.515c-.33-1.02.211-2.129 1.232-2.458 1.02-.329 2.13.209 2.461 1.229l.842 2.515 5.011-1.677-.839-2.517c-.403-1.238.484-2.553 1.843-2.553.819 0 1.585.509 1.85 1.326l.841 2.517 2.431-.81c1.02-.33 2.131.211 2.461 1.229.332 1.018-.21 2.126-1.23 2.456l-2.433.809 1.622 4.823 2.433-.809c1.242-.401 2.557.484 2.557 1.838 0 .819-.51 1.583-1.328 1.847m-8.992-6.428l-5.01 1.675 1.619 4.828 5.011-1.674-1.62-4.829z"
			></path></svg
		>
		<p>Tzu Shao<br />Bryan Liu :&#41;</p>
	</aside>
	<nav>
		<h6 class="footer-title">Social</h6>
		<div class="grid grid-flow-col gap-4">
			<a
				><svg
					xmlns="http://www.w3.org/2000/svg"
					width="24"
					height="24"
					viewBox="0 0 24 24"
					class="fill-current"
					><path
						d="M24 4.557c-.883.392-1.832.656-2.828.775 1.017-.609 1.798-1.574 2.165-2.724-.951.564-2.005.974-3.127 1.195-.897-.957-2.178-1.555-3.594-1.555-3.179 0-5.515 2.966-4.797 6.045-4.091-.205-7.719-2.165-10.148-5.144-1.29 2.213-.669 5.108 1.523 6.574-.806-.026-1.566-.247-2.229-.616-.054 2.281 1.581 4.415 3.949 4.89-.693.188-1.452.232-2.224.084.626 1.956 2.444 3.379 4.6 3.419-2.07 1.623-4.678 2.348-7.29 2.04 2.179 1.397 4.768 2.212 7.548 2.212 9.142 0 14.307-7.721 13.995-14.646.962-.695 1.797-1.562 2.457-2.549z"
					></path></svg
				></a
			>
			<a
				><svg
					xmlns="http://www.w3.org/2000/svg"
					width="24"
					height="24"
					viewBox="0 0 24 24"
					class="fill-current"
					><path
						d="M19.615 3.184c-3.604-.246-11.631-.245-15.23 0-3.897.266-4.356 2.62-4.385 8.816.029 6.185.484 8.549 4.385 8.816 3.6.245 11.626.246 15.23 0 3.897-.266 4.356-2.62 4.385-8.816-.029-6.185-.484-8.549-4.385-8.816zm-10.615 12.816v-8l8 3.993-8 4.007z"
					></path></svg
				></a
			>
			<a
				><svg
					xmlns="http://www.w3.org/2000/svg"
					width="24"
					height="24"
					viewBox="0 0 24 24"
					class="fill-current"
					><path
						d="M9 8h-3v4h3v12h5v-12h3.642l.358-4h-4v-1.667c0-.955.192-1.333 1.115-1.333h2.885v-5h-3.808c-3.596 0-5.192 1.583-5.192 4.615v3.385z"
					></path></svg
				></a
			>
		</div>
	</nav>
</footer>

<style>
	.embla {
		overflow: hidden;
	}
	.embla__container {
		display: flex;
	}
	.embla__slide {
		flex: 0 0 100%;
		min-width: 0;
	}
</style>
