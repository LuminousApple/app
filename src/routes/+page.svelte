<script lang="ts">
	import './layout.css';
	import logo from '$lib/assets/favicon.jpg';
</script>

<section class="sticky top-0 flex flex-row justify-between bg-black px-10 font-sans">
	<div class="py-5">
		<img src={logo} alt="logo" class="h-10 w-10 rounded" />
	</div>
	<div class="flex gap-4 py-8">
		<a href="https://github.com/LuminousApple" class="text-white no-underline">Github</a>
		<a href="#about" class="text-white no-underline">About</a>
	</div>
</section>

<hr class="mt-* w-full border-t border-amber-400 shadow-2xl" />

<section class="flex min-h-screen flex-col items-center gap-8 bg-black pt-80 font-sans">
	<h1 class="font-mono text-5xl font-extrabold tracking-tight text-yellow-500">Luminous Apple</h1>
	<a
		href="https://github.com/LuminousApple"
		class="m-3 rounded-lg bg-amber-400 p-2 px-5 py-2.5 font-bold text-black shadow-lg shadow-amber-400/50 transition-all duration-300 hover:scale-105"
		>Github Org ↗&#xFE0E;</a
	>
</section>
