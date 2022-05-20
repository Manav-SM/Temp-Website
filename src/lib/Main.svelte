<script lang="ts">
	import { fade } from 'svelte/transition';
	import Footer from './Footer.svelte';
</script>

<svelte:head>
	<link rel="icon" href="./favicon2.png" type="image/x-icon" />
	<title>Home</title>
</svelte:head>

<main in:fade>
	<div class="hero min-h-screen p-10 sm:p-36">
		<div class="flex-col hero-content lg:flex-row-reverse mr-4 gap-x-4">
			<img
				src="./portrait.jpg"
				alt="@Portrait"
				class="hidden sm:block w-60 h-60 avatar mask mask-squircle cursor-move transform-gpu hover:scale-95 transition-transform"
			/>
			<div class="select-none">
				<h1 class="mb-5 text-2xl font-bold sm:text-5xl">
					👋, I'm <span
						class="text-transparent bg-clip-text bg-gradient-to-tr from-indigo-600 to-purple-200"
						>Manav</span
					>
				</h1>
				<p class="mb-5 text-xs sm:text-lg">
					Programmer, <span
						class="text-transparent bg-clip-text bg-gradient-to-tr from-red-500 to-purple-300"
						>IoT enthusiast
					</span>
					and
					<span class="text-transparent bg-clip-text bg-gradient-to-tr from-red-500 to-purple-300">
						a gamer
					</span>from Mumbai.
				</p>
				<Footer />
			</div>
		</div>
	</div>
</main>
