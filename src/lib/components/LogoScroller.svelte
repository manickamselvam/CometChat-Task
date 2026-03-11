<script>
	const logos = [
		'/brand-logos/haleon.svg',
		'/brand-logos/kahoot.svg',
		'/brand-logos/shaadi.svg',
		'/brand-logos/endeavor.svg',
		'/brand-logos/nobrocker.svg',
		'/brand-logos/Konecta.png'
	];
</script>

<section class="bg-[#0A0914] px-4 py-14 md:px-6 md:py-20">
	<div class="mx-auto w-full max-w-7xl md:w-[80%]">
		<div class="relative">
			<!-- MAIN BORDERS -->
			<div class="absolute top-0 right-0 left-0 h-px bg-[rgba(250,250,255,0.1)]"></div>

			<div class="absolute right-0 bottom-0 left-0 h-px bg-[rgba(250,250,255,0.1)]"></div>
			<div class="absolute top-0 bottom-0 left-0 w-px bg-[rgba(250,250,255,0.1)]"></div>
			<div class="absolute top-0 right-0 bottom-0 w-px bg-[rgba(250,250,255,0.1)]"></div>

			<!-- EXTENDED HORIZONTAL LINES (HIDDEN ON MOBILE) -->
			<div
				class="absolute top-0 right-full hidden h-px w-20 md:block"
				style="background: linear-gradient(90deg, rgba(250,250,255,0) 0%, rgba(250,250,255,0.1) 30%, rgba(250,250,255,0.1) 100%);"
			></div>

			<div
				class="absolute top-0 left-full hidden h-px w-20 md:block"
				style="background: linear-gradient(90deg, rgba(250,250,255,0.1) 0%, rgba(250,250,255,0.1) 70%, rgba(250,250,255,0) 100%);"
			></div>

			<div
				class="absolute right-full bottom-0 hidden h-px w-20 md:block"
				style="background: linear-gradient(90deg, rgba(250,250,255,0) 0%, rgba(250,250,255,0.1) 30%, rgba(250,250,255,0.1) 100%);"
			></div>

			<div
				class="absolute bottom-0 left-full hidden h-px w-20 md:block"
				style="background: linear-gradient(90deg, rgba(250,250,255,0.1) 0%, rgba(250,250,255,0.1) 70%, rgba(250,250,255,0) 100%);"
			></div>

			<!-- CORNER DOTS -->
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

			<!-- AUTO SCROLL CONTENT -->
			<div class="overflow-hidden py-8 md:h-34 md:py-12">
				<div class="animate-scroll flex w-max gap-10 md:gap-16">
					{#each [...logos, ...logos] as logo, i (i)}
						<img src={logo} alt="brand logo" class="h-6 opacity-70 grayscale md:h-8" />
					{/each}
				</div>
			</div>
		</div>
	</div>
</section>

<style>
	@keyframes scroll {
		from {
			transform: translateX(0);
		}
		to {
			transform: translateX(-50%);
		}
	}

	.animate-scroll {
		animation: scroll 10s linear infinite;
	}
</style>
