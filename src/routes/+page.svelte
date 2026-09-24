<script lang="ts">
	import './layout.css';
	import logo from '$lib/assets/favicon.jpg';

	// Optional: Data structure to keep the markup clean
	const members = [
		{ name: 'Crunchy', role: 'Developer', github: 'https://github.com/CrunchysPixelPillow' },
		{ name: 'Ocean', role: 'Developer', github: 'https://github.com/BlueOceanVale' },
		{ name: 'Mishra', role: 'Developer', github: 'https://github.com/ayushmishra34er' }
	];
</script>

<!-- Navigation Bar -->
<header
	class="sticky top-0 z-50 flex items-center justify-between border-b border-amber-400/20 bg-black/90 px-6 py-4 font-sans backdrop-blur-md md:px-10"
>
	<div class="flex items-center gap-3">
		<img
			src={logo}
			alt="Luminous Apple Logo"
			class="h-10 w-10 rounded-lg border border-amber-400/30"
		/>
	</div>
	<nav class="flex items-center gap-6 text-sm font-medium">
		<a
			href="https://github.com/LuminousApple"
			target="_blank"
			rel="noopener noreferrer"
			class="text-neutral-300 no-underline transition-colors hover:text-amber-400">Github</a
		>
		<a href="#about" class="text-neutral-300 no-underline transition-colors hover:text-amber-400"
			>About</a
		>
	</nav>
</header>

<hr class="w-full border-t border-amber-400 shadow-[0_0_15px_rgba(251,191,36,0.3)]" />

<!-- Hero Section -->
<section
	class="flex min-h-[75vh] flex-col items-center justify-center gap-6 bg-black px-4 text-center font-sans"
>
	<h1
		class="font-mono text-5xl font-extrabold tracking-tight text-amber-400 drop-shadow-[0_0_25px_rgba(251,191,36,0.2)] md:text-7xl"
	>
		Luminous Apple
	</h1>
	<p class="max-w-md text-sm text-neutral-400 md:text-base">
		Building open-source software and tools with precision.
	</p>
	<a
		href="https://github.com/LuminousApple"
		target="_blank"
		rel="noopener noreferrer"
		class="rounded-lg bg-amber-400 px-6 py-2.5 font-bold text-black shadow-lg shadow-amber-400/40 transition-all duration-300 hover:scale-105 hover:bg-amber-300"
	>
		Github Org ↗&#xFE0E;
	</a>
</section>

<!-- Members Section -->
<section class="bg-black px-6 py-16 font-sans md:px-12">
	<div class="mx-auto max-w-6xl">
		<h2 class="mb-8 text-2xl font-bold tracking-tight text-amber-400">Our Members</h2>
		<div class="grid grid-cols-1 gap-6 sm:grid-cols-2 lg:grid-cols-3">
			{#each members as member}
				<div
					class="group flex flex-col items-center gap-2 rounded-xl border border-neutral-800 bg-neutral-900/50 p-6 text-center transition-all duration-300 hover:border-amber-400/60 hover:bg-neutral-900/80 hover:shadow-lg hover:shadow-amber-400/10"
				>
					<!-- Placeholder Avatar -->
					<div
						class="flex h-14 w-14 items-center justify-center rounded-full border border-amber-400/20 bg-neutral-800 font-bold text-amber-400 transition-colors group-hover:border-amber-400"
					>
						{member.name[0]}
					</div>
					<h3 class="text-lg font-bold text-white transition-colors group-hover:text-amber-300">
						{member.name}
					</h3>
					<span
						class="rounded-full bg-amber-400/10 px-2.5 py-0.5 text-xs font-medium text-amber-400/80"
						>{member.role}</span
					>
				</div>
			{/each}
		</div>
	</div>
</section>
