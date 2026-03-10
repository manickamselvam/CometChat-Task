<script>
	const navItems = ['Platform', 'Solution', 'Developers', 'Resources', 'Pricing'];
</script>

<nav class="w-full bg-[#0A0914]">
	<div class="mx-auto flex items-center justify-between px-8 py-4">
		<!-- Left : Logo -->
		<div class="flex items-center">
			<img src="/Logo.svg" alt="CometChat Logo" />
		</div>

		<!-- Center : Navigation -->

		<ul class="hidden items-center gap-8 text-sm font-medium text-gray-700 md:flex">
			{#each navItems as item (item)}
				<li
					class="h-5 cursor-pointer font-['Satoshi_Variable'] text-sm leading-[140%] font-semibold tracking-[0.02em] text-[#FAFAFF] opacity-[0.84] transition hover:text-blue-400"
				>
					{item}
				</li>
			{/each}
		</ul>

		<!-- Right : Actions -->
		<div class="flex items-center gap-4">
			<button
				class="h-5 cursor-pointer font-['Satoshi_Variable'] text-sm leading-[140%] font-semibold tracking-[0.02em] text-[#FAFAFF] opacity-[0.84] transition hover:text-blue-400"
			>
				Login
			</button>

			<button
				class="flex h-9 cursor-pointer items-center justify-center gap-2.5 rounded-[10px] bg-[#6852D6] px-3 py-2 text-sm font-medium text-white"
			>
				<span
					class="h-5 font-['Satoshi_Variable'] text-sm leading-[140%] font-semibold tracking-[0.02em] text-[#FCFCFE]"
					>Schedule a demo</span
				>
			</button>
		</div>
	</div>
</nav>
