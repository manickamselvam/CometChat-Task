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

<section class="bg-[#0A0914] px-6 py-20">
	<div class="mx-auto w-[80%] max-w-7xl text-center">
		<p
			class="h-5.75 pb-[30px] text-center font-['Satoshi_Variable'] text-[22px] leading-[106%] font-semibold tracking-normal text-[#6852D6]"
		>
			Chat integration options
		</p>

		<h2
			class="h-12.75 pb-[60px] text-center font-['Satoshi_Variable'] text-[48px] leading-[106%] font-semibold tracking-normal text-[#FAFAFF]"
		>
			Your launch, your way. Done right.
		</h2>

		<p
			class="h-13 pb-[120px] text-center font-['Satoshi_Variable'] text-[22px] leading-[120%] font-medium tracking-[0.5%] text-[#FAFAFF] opacity-74"
		>
			Start with what gets you to production fastest — or matches your needs the best. <br /> Swap it
			out or level it up later.
		</p>

		<!-- GRID FRAME -->
		<div class="relative">
			<!-- 4 SIDE BORDERS (top, bottom, left, right) -->
			<div class="absolute top-0 right-0 left-0 h-px bg-[rgba(250,250,255,0.1)]"></div>
			<div class="absolute right-0 bottom-0 left-0 h-px bg-[rgba(250,250,255,0.1)]"></div>
			<div class="absolute top-0 bottom-0 left-0 w-px bg-[rgba(250,250,255,0.1)]"></div>
			<div class="absolute top-0 right-0 bottom-0 w-px bg-[rgba(250,250,255,0.1)]"></div>

			<!-- INTERNAL VERTICAL DIVIDERS -->
			<div class="absolute top-0 bottom-0 left-1/3 w-px bg-[rgba(250,250,255,0.1)]"></div>
			<div class="absolute top-0 bottom-0 left-2/3 w-px bg-[rgba(250,250,255,0.1)]"></div>

			<!-- EXTENDED HORIZONTAL LINES FROM CORNER DOTS -->
			<!-- Top Left - fades left -->
			<div
				class="absolute top-0 right-full h-px w-20"
				style="background: linear-gradient(90deg, rgba(250, 250, 255, 0) 0%, rgba(250, 250, 255, 0.1) 30%, rgba(250, 250, 255, 0.1) 100%);"
			></div>
			<!-- Top Right - fades right -->
			<div
				class="absolute top-0 left-full h-px w-20"
				style="background: linear-gradient(90deg, rgba(250, 250, 255, 0.1) 0%, rgba(250, 250, 255, 0.1) 70%, rgba(250, 250, 255, 0) 100%);"
			></div>
			<!-- Bottom Left - fades left -->
			<div
				class="absolute right-full bottom-0 h-px w-20"
				style="background: linear-gradient(90deg, rgba(250, 250, 255, 0) 0%, rgba(250, 250, 255, 0.1) 30%, rgba(250, 250, 255, 0.1) 100%);"
			></div>
			<!-- Bottom Right - fades right -->
			<div
				class="absolute bottom-0 left-full h-px w-20"
				style="background: linear-gradient(90deg, rgba(250, 250, 255, 0.1) 0%, rgba(250, 250, 255, 0.1) 70%, rgba(250, 250, 255, 0) 100%);"
			></div>

			<!-- CORNER DOTS (4 corners) -->
			<div
				class="absolute top-0 left-0 z-10 h-4 w-4 -translate-x-1/2 -translate-y-1/2 rounded-full border border-[#FAFAFF1A] bg-[#0A0914]"
			></div>
			<div
				class="absolute top-0 right-0 z-10 h-4 w-4 translate-x-1/2 -translate-y-1/2 rounded-full border border-[#FAFAFF1A] bg-[#0A0914]"
			></div>
			<div
				class="absolute bottom-0 left-0 z-10 h-4 w-4 -translate-x-1/2 translate-y-1/2 rounded-full border border-[#FAFAFF1A] bg-[#0A0914]"
			></div>
			<div
				class="absolute right-0 bottom-0 z-10 h-4 w-4 translate-x-1/2 translate-y-1/2 rounded-full border border-[#FAFAFF1A] bg-[#0A0914]"
			></div>

			<!-- INTERNAL DOTS (top middle dividers) -->
			<div
				class="absolute top-0 left-1/3 z-10 h-4 w-4 -translate-x-1/2 -translate-y-1/2 rounded-full border border-[#FAFAFF1A] bg-[#0A0914]"
			></div>
			<div
				class="absolute top-0 left-2/3 z-10 h-4 w-4 -translate-x-1/2 -translate-y-1/2 rounded-full border border-[#FAFAFF1A] bg-[#0A0914]"
			></div>

			<!-- INTERNAL DOTS (bottom middle dividers) -->
			<div
				class="absolute bottom-0 left-1/3 z-10 h-4 w-4 -translate-x-1/2 translate-y-1/2 rounded-full border border-[#FAFAFF1A] bg-[#0A0914]"
			></div>
			<div
				class="absolute bottom-0 left-2/3 z-10 h-4 w-4 -translate-x-1/2 translate-y-1/2 rounded-full border border-[#FAFAFF1A] bg-[#0A0914]"
			></div>

			<!-- CARDS -->

			<div class="grid text-left md:grid-cols-3">
				{#each options as option (option.title)}
					<div class="p-7">
						<img src={option.icon} alt="icon" class="h-16 w-16" />
						<div>
							<h3
								class="mt-[75px] font-['Satoshi_Variable'] text-[24px] leading-[106%] font-semibold tracking-normal text-[#FAFAFF]"
							>
								{option.title}
							</h3>

							<p
								class="py-[15px] font-['Satoshi_Variable'] text-[18px] leading-[120%] font-medium tracking-[0.5%] text-[#FAFAFF] opacity-74"
							>
								{option.desc}
							</p>

							<a
								href="#"
								class="font-['Satoshi_Variable'] text-[18px] leading-[112%] font-semibold tracking-normal text-[#6852D6]"
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
