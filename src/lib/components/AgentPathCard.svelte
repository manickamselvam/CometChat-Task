<script>
	export let icon;
	export let heading;
	export let items = [];
	export let image;
</script>

<div
	class="rounded-3xl p-px"
	style="background: radial-gradient(53.51% 100% at 53.51% 0%, rgba(250,250,255,0.3) 0%, rgba(250,250,255,0.1) 100%);"
>
	<div
		class="flex h-161.25 flex-col gap-6 rounded-3xl bg-[#0A0914] p-8"
	>
		<!-- TOP ICON -->
		<img src={icon} alt="icon" class="h-10 w-10" />

		<!-- HEADING -->
		<h3 class="font-['Satoshi_Variable'] text-[24px] font-semibold leading-[106%] text-[#FAFAFF]">
			{heading}
		</h3>

		<!-- LIST ITEMS -->
		<div class="space-y-3">
			{#each items as item (item)}
				<div class="flex items-start gap-3">
					<img src="/star.svg" alt="star" class="mt-1 h-4 w-4 shrink-0" />
					<p class="font-['Satoshi_Variable'] text-[18px] font-medium leading-[120%] text-[#FAFAFF] opacity-70">
						{item}
					</p>
				</div>
			{/each}
		</div>

		<!-- LEARN MORE -->
		<a href="#" class="font-['Satoshi_Variable'] text-[18px] font-semibold text-[#6852D6]">
			Learn more
		</a>

		<!-- IMAGE -->
		<img src={image} alt="card preview" class="mt-4 w-full rounded-lg object-cover" />
	</div>
</div>