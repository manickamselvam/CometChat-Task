<script>
	const navItems = ['Platform', 'Solution', 'Developers', 'Resources', 'Pricing'];
	let menuOpen = false;

	const toggleMenu = () => {
		menuOpen = !menuOpen;
	};
</script>

<nav class="relative w-full bg-[#0A0914]">
	<div class="mx-auto flex items-center justify-between px-4 py-4 md:px-8">
		<!-- Logo -->
		<a href="/" class="flex items-center">
			<img src="/Logo.svg" alt="CometChat" class="h-6 md:h-8" loading="eager" />
		</a>

		<!-- Desktop Navigation -->
		<ul class="hidden items-center gap-8 lg:flex">
			{#each navItems as item (item)}
				<li>
					<a
						href="#"
						class="cursor-pointer text-sm font-semibold text-[#FAFAFF] opacity-[0.84] transition-colors hover:text-blue-400"
					>
						{item}
					</a>
				</li>
			{/each}
		</ul>

		<!-- Right Actions -->
		<div class="flex items-center gap-4">
			<!-- Login -->
			<button
				class="cursor-pointer text-sm font-semibold text-[#FAFAFF] opacity-[0.84] transition-colors hover:text-blue-400"
			>
				Login
			</button>

			<!-- Schedule Demo -->
			<button
				class="hidden h-9 items-center justify-center gap-2.5 rounded-[10px] bg-[#6852D6] px-3 py-2 text-sm font-medium text-white transition hover:bg-[#5742c4] lg:flex"
			>
				Schedule a demo
			</button>

			<!-- Mobile Menu Button -->
			<button
				class="text-white lg:hidden"
				aria-label="Toggle menu"
				aria-expanded={menuOpen}
				on:click={toggleMenu}
			>
				<img src="/mobilemenu.svg" alt="Menu icon" class="h-6 w-6" />
			</button>
		</div>
	</div>

	<!-- Mobile Menu -->
	{#if menuOpen}
		<div class="space-y-5 bg-[#0A0914] px-6 py-6 lg:hidden">
			{#each navItems as item (item)}
				<a
					href="#"
					class="block cursor-pointer text-sm font-semibold text-[#FAFAFF] opacity-[0.84] transition-colors hover:text-blue-400"
				>
					{item}
				</a>
			{/each}

			<button
				class="mt-4 h-10 w-full rounded-[10px] bg-[#6852D6] font-semibold text-white transition hover:bg-[#5742c4]"
			>
				Schedule a demo
			</button>
		</div>
	{/if}
</nav>
