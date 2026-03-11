<script>
	const navItems = ['Platform', 'Solution', 'Developers', 'Resources', 'Pricing'];
	let menuOpen = false;
</script>

<nav class="relative w-full bg-[#0A0914]">
	<div class="mx-auto flex items-center justify-between px-4 py-4 md:px-8">
		<!-- Logo -->
		<div class="flex items-center">
			<img src="/Logo.svg" alt="CometChat Logo" class="h-6 md:h-8" />
		</div>

		<!-- Desktop Navigation -->
		<ul class="hidden items-center gap-8 lg:flex">
			{#each navItems as item (item)}
				<li
					class="cursor-pointer font-['Satoshi_Variable'] text-sm font-semibold text-[#FAFAFF] opacity-[0.84] transition hover:text-blue-400"
				>
					{item}
				</li>
			{/each}
		</ul>

		<!-- Right Actions -->
		<div class="flex items-center gap-4">
			<!-- Login (always visible) -->
			<button
				class="cursor-pointer font-['Satoshi_Variable'] text-sm font-semibold text-[#FAFAFF] opacity-[0.84] hover:text-blue-400"
			>
				Login
			</button>

			<!-- Schedule Demo (desktop only) -->
			<button
				class="hidden h-9 items-center justify-center gap-2.5 rounded-[10px] bg-[#6852D6] px-3 py-2 text-sm font-medium text-white lg:flex"
			>
				Schedule a demo
			</button>

			<!-- Hamburger (mobile only) -->
			<button class="text-2xl text-white lg:hidden" on:click={() => (menuOpen = !menuOpen)}>
				<img src="/mobilemenu.svg" alt="mobile menu icon" />
			</button>
		</div>
	</div>

	<!-- Mobile Menu -->
	{#if menuOpen}
		<div class="space-y-5 border-t border-gray-800 bg-[#0A0914] px-6 py-6 lg:hidden">
			{#each navItems as item (item)}
				<div
					class="cursor-pointer font-['Satoshi_Variable'] text-sm font-semibold text-[#FAFAFF] opacity-[0.84] hover:text-blue-400"
				>
					{item}
				</div>
			{/each}

			<button class="mt-4 h-10 w-full rounded-[10px] bg-[#6852D6] font-semibold text-white">
				Schedule a demo
			</button>
		</div>
	{/if}
</nav>