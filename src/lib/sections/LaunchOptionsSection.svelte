<script>
	const options = [
		{
			icon: '/chat-builder-icon.svg',
			title: 'Chat Builder',
			desc: 'The fastest way to go live.',
			link: 'Try Builder'
		},
		{
			icon: '/Ui-kit-icon.svg',
			title: 'UI Kits',
			desc: 'Production-ready components with full flexibility.',
			link: 'Try Builder'
		},
		{
			icon: '/sdk-icon.svg',
			title: 'SDKs & APIs',
			desc: 'The toolbox for when you want total control.',
			link: 'Try Builder'
		}
	];
</script>

<section class="bg-[#0A0914] px-6 py-12 sm:py-16 lg:py-20">
	<div class="mx-auto w-full max-w-7xl text-center sm:w-[90%] lg:w-[80%]">
		<p
			class="pb-6 text-center font-['Satoshi_Variable'] text-[18px] leading-[106%] font-semibold tracking-normal text-[#6852D6] sm:pb-8 sm:text-[20px] lg:text-[22px]"
		>
			Chat integration options
		</p>

		<h2
			class="pb-8 text-center font-['Satoshi_Variable'] text-[32px] leading-[106%] font-semibold tracking-normal text-[#FAFAFF] sm:pb-10 sm:text-[40px] lg:pb-[60px] lg:text-[48px]"
		>
			Your launch, your way. Done right.
		</h2>

		<p
			class="pb-12 text-center font-['Satoshi_Variable'] text-[18px] leading-[120%] font-medium tracking-[0.5%] text-[#FAFAFF] opacity-74 sm:pb-16 sm:text-[20px] lg:pb-[120px] lg:text-[22px]"
		>
			Start with what gets you to production fastest — or matches your needs the best. <br class="hidden sm:block" /> Swap it
			out or level it up later.
		</p>

		<!-- GRID FRAME -->
		<div class="relative">
			<!-- 4 SIDE BORDERS (top, bottom, left, right) -->
			<div class="absolute top-0 right-0 left-0 h-px bg-[rgba(250,250,255,0.1)]"></div>
			<div class="absolute right-0 bottom-0 left-0 h-px bg-[rgba(250,250,255,0.1)]"></div>
			<div class="absolute top-0 bottom-0 left-0 w-px bg-[rgba(250,250,255,0.1)]"></div>
			<div class="absolute top-0 right-0 bottom-0 w-px bg-[rgba(250,250,255,0.1)]"></div>

			<!-- INTERNAL VERTICAL DIVIDERS - Hidden on mobile, shown on md+ -->
			<div class="absolute top-0 bottom-0 left-1/3 hidden w-px bg-[rgba(250,250,255,0.1)] md:block"></div>
			<div class="absolute top-0 bottom-0 left-2/3 hidden w-px bg-[rgba(250,250,255,0.1)] md:block"></div>

			<!-- INTERNAL HORIZONTAL DIVIDERS - Shown on mobile between stacked cards -->
			<div class="absolute right-0 left-0 top-1/3 h-px bg-[rgba(250,250,255,0.1)] md:hidden"></div>
			<div class="absolute right-0 left-0 top-2/3 h-px bg-[rgba(250,250,255,0.1)] md:hidden"></div>

			<!-- EXTENDED HORIZONTAL LINES FROM CORNER DOTS - Hidden on mobile -->
			<div
				class="absolute top-0 right-full hidden h-px w-20 sm:block"
				style="background: linear-gradient(90deg, rgba(250, 250, 255, 0) 0%, rgba(250, 250, 255, 0.1) 30%, rgba(250, 250, 255, 0.1) 100%);"
			></div>
			<div
				class="absolute top-0 left-full hidden h-px w-20 sm:block"
				style="background: linear-gradient(90deg, rgba(250, 250, 255, 0.1) 0%, rgba(250, 250, 255, 0.1) 70%, rgba(250, 250, 255, 0) 100%);"
			></div>
			<div
				class="absolute right-full bottom-0 hidden h-px w-20 sm:block"
				style="background: linear-gradient(90deg, rgba(250, 250, 255, 0) 0%, rgba(250, 250, 255, 0.1) 30%, rgba(250, 250, 255, 0.1) 100%);"
			></div>
			<div
				class="absolute bottom-0 left-full hidden h-px w-20 sm:block"
				style="background: linear-gradient(90deg, rgba(250, 250, 255, 0.1) 0%, rgba(250, 250, 255, 0.1) 70%, rgba(250, 250, 255, 0) 100%);"
			></div>

			<!-- CORNER DOTS (4 corners) -->
			<div
				class="absolute top-0 left-0 z-10 h-3 w-3 -translate-x-1/2 -translate-y-1/2 rounded-full border border-[#FAFAFF1A] bg-[#0A0914] sm:h-4 sm:w-4"
			></div>
			<div
				class="absolute top-0 right-0 z-10 h-3 w-3 translate-x-1/2 -translate-y-1/2 rounded-full border border-[#FAFAFF1A] bg-[#0A0914] sm:h-4 sm:w-4"
			></div>
			<div
				class="absolute bottom-0 left-0 z-10 h-3 w-3 -translate-x-1/2 translate-y-1/2 rounded-full border border-[#FAFAFF1A] bg-[#0A0914] sm:h-4 sm:w-4"
			></div>
			<div
				class="absolute right-0 bottom-0 z-10 h-3 w-3 translate-x-1/2 translate-y-1/2 rounded-full border border-[#FAFAFF1A] bg-[#0A0914] sm:h-4 sm:w-4"
			></div>

			<!-- INTERNAL DOTS (top middle dividers) - Hidden on mobile -->
			<div
				class="absolute top-0 left-1/3 z-10 hidden h-4 w-4 -translate-x-1/2 -translate-y-1/2 rounded-full border border-[#FAFAFF1A] bg-[#0A0914] md:block"
			></div>
			<div
				class="absolute top-0 left-2/3 z-10 hidden h-4 w-4 -translate-x-1/2 -translate-y-1/2 rounded-full border border-[#FAFAFF1A] bg-[#0A0914] md:block"
			></div>

			<!-- INTERNAL DOTS (bottom middle dividers) - Hidden on mobile -->
			<div
				class="absolute bottom-0 left-1/3 z-10 hidden h-4 w-4 -translate-x-1/2 translate-y-1/2 rounded-full border border-[#FAFAFF1A] bg-[#0A0914] md:block"
			></div>
			<div
				class="absolute bottom-0 left-2/3 z-10 hidden h-4 w-4 -translate-x-1/2 translate-y-1/2 rounded-full border border-[#FAFAFF1A] bg-[#0A0914] md:block"
			></div>

			<!-- MOBILE HORIZONTAL DOTS (left and right at 1/3 and 2/3) - Shown only on mobile -->
			<div
				class="absolute top-1/3 left-0 z-10 h-3 w-3 -translate-x-1/2 -translate-y-1/2 rounded-full border border-[#FAFAFF1A] bg-[#0A0914] md:hidden"
			></div>
			<div
				class="absolute top-1/3 right-0 z-10 h-3 w-3 translate-x-1/2 -translate-y-1/2 rounded-full border border-[#FAFAFF1A] bg-[#0A0914] md:hidden"
			></div>
			<div
				class="absolute top-2/3 left-0 z-10 h-3 w-3 -translate-x-1/2 -translate-y-1/2 rounded-full border border-[#FAFAFF1A] bg-[#0A0914] md:hidden"
			></div>
			<div
				class="absolute top-2/3 right-0 z-10 h-3 w-3 translate-x-1/2 -translate-y-1/2 rounded-full border border-[#FAFAFF1A] bg-[#0A0914] md:hidden"
			></div>

			<!-- CARDS -->
			<div class="grid text-left md:grid-cols-3">
				{#each options as option (option.title)}
					<div class="p-5 sm:p-6 lg:p-7">
						<img src={option.icon} alt="icon" class="h-12 w-12 sm:h-14 sm:w-14 lg:h-16 lg:w-16" />
						<div>
							<h3
								class="mt-12 font-['Satoshi_Variable'] text-[20px] leading-[106%] font-semibold tracking-normal text-[#FAFAFF] sm:mt-16 sm:text-[22px] lg:mt-[75px] lg:text-[24px]"
							>
								{option.title}
							</h3>

							<p
								class="py-3 font-['Satoshi_Variable'] text-[16px] leading-[120%] font-medium tracking-[0.5%] text-[#FAFAFF] opacity-74 sm:py-4 sm:text-[17px] lg:py-[15px] lg:text-[18px]"
							>
								{option.desc}
							</p>

							<a
								href="#"
								class="font-['Satoshi_Variable'] text-[16px] leading-[112%] font-semibold tracking-normal text-[#6852D6] sm:text-[17px] lg:text-[18px]"
							>
								{option.link}
							</a>
						</div>
					</div>
				{/each}
			</div>
		</div>
	</div>
</section>