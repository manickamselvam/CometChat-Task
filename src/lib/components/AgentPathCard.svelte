<script>
	export let icon;
	export let heading;
	export let items = [];
	export let image;
</script>

<div
	class="rounded-2xl p-px sm:rounded-3xl"
	style="background: radial-gradient(53.51% 100% at 53.51% 0%, rgba(250,250,255,0.3) 0%, rgba(250,250,255,0.1) 100%);"
>
	<div
		class="flex min-h-[400px] flex-col gap-4 rounded-2xl bg-[#0A0914] p-6 sm:min-h-[500px] sm:gap-6 sm:rounded-3xl sm:p-8"
	>
		<!-- TOP ICON -->
		<img src={icon} alt="icon" class="h-8 w-8 sm:h-10 sm:w-10" />

		<!-- HEADING -->
		<h3
			class="font-['Satoshi_Variable'] text-[20px] leading-[106%] font-semibold text-[#FAFAFF] sm:text-[22px] lg:text-[24px]"
		>
			{heading}
		</h3>

		<!-- LIST ITEMS -->
		<div class="space-y-2.5 sm:space-y-3">
			{#each items as item (item)}
				<div class="flex items-start gap-2.5 sm:gap-3">
					<img
						src="/star.svg"
						alt="star"
						class="mt-0.5 h-3.5 w-3.5 shrink-0 sm:mt-1 sm:h-4 sm:w-4"
					/>
					<p
						class="font-['Satoshi_Variable'] text-[16px] leading-[120%] font-medium text-[#FAFAFF] opacity-70 sm:text-[17px] lg:text-[18px]"
					>
						{item}
					</p>
				</div>
			{/each}
		</div>

		<!-- LEARN MORE -->
		<a
			href="#"
			class="font-['Satoshi_Variable'] text-[16px] font-semibold text-[#6852D6] sm:text-[17px] lg:text-[18px]"
		>
			Learn more
		</a>

		<!-- IMAGE -->
		<img src={image} alt="card preview" class="mt-2 w-full rounded-lg object-cover sm:mt-4" />
	</div>
</div>
