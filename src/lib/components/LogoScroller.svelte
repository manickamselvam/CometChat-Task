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

<section class="bg-[#0A0914] px-6 py-20">
	<div class="mx-auto w-[80%] max-w-7xl">
		<div class="relative">
			<!-- 4 SIDE BORDERS -->
			<div class="absolute top-0 right-0 left-0 h-px w-full bg-[rgba(250,250,255,0.1)]"></div>
			<div class="absolute right-0 bottom-0 left-0 h-px bg-[rgba(250,250,255,0.1)]"></div>
			<div class="absolute top-0 bottom-0 left-0 w-px bg-[rgba(250,250,255,0.1)]"></div>
			<div class="absolute top-0 right-0 bottom-0 w-px bg-[rgba(250,250,255,0.1)]"></div>

			<!-- EXTENDED HORIZONTAL LINES FROM DOTS -->
			<!-- Top Left - solid at dot (right), fades left -->
			<div
				class="absolute top-0 right-full h-px w-20"
				style="background: linear-gradient(90deg, rgba(250, 250, 255, 0) 0%, rgba(250, 250, 255, 0.1) 30%, rgba(250, 250, 255, 0.1) 100%);"
			></div>

			<!-- Top Right - solid at dot (left), fades right -->
			<div
				class="absolute top-0 left-full h-px w-20"
				style="background: linear-gradient(90deg, rgba(250, 250, 255, 0.1) 0%, rgba(250, 250, 255, 0.1) 70%, rgba(250, 250, 255, 0) 100%);"
			></div>

			<!-- Bottom Left - solid at dot (right), fades left -->
			<div
				class="absolute right-full bottom-0 h-px w-20"
				style="background: linear-gradient(90deg, rgba(250, 250, 255, 0) 0%, rgba(250, 250, 255, 0.1) 30%, rgba(250, 250, 255, 0.1) 100%);"
			></div>

			<!-- Bottom Right - solid at dot (left), fades right -->
			<div
				class="absolute bottom-0 left-full h-px w-20"
				style="background: linear-gradient(90deg, rgba(250, 250, 255, 0.1) 0%, rgba(250, 250, 255, 0.1) 70%, rgba(250, 250, 255, 0) 100%);"
			></div>

			<!-- 4 CORNER DOTS -->
			<!-- w-4 h-4 opacity-100 border border-[#FAFAFF1A] bg-[#0A0914] -->
			<div
				class="absolute top-0 left-0 z-10 h-4 w-4 -translate-x-1/2 -translate-y-1/2 rounded-full border border-[#FAFAFF1A] bg-[#0A0914] opacity-100"
			></div>
			<div
				class="absolute top-0 right-0 z-10 h-4 w-4 translate-x-1/2 -translate-y-1/2 rounded-full border border-[#FAFAFF1A] bg-[#0A0914] opacity-100"
			></div>
			<div
				class="absolute bottom-0 left-0 z-10 h-4 w-4 -translate-x-1/2 translate-y-1/2 rounded-full border border-[#FAFAFF1A] bg-[#0A0914] opacity-100"
			></div>
			<div
				class="absolute right-0 bottom-0 z-10 h-4 w-4 translate-x-1/2 translate-y-1/2 rounded-full border border-[#FAFAFF1A] bg-[#0A0914] opacity-100"
			></div>

			<!-- AUTO-SCROLLING CONTENT -->
			<div class="h-34 overflow-hidden py-12">
				<div class="animate-scroll flex w-max gap-16">
					{#each [...logos, ...logos] as logo, i (i)}
						<img src={logo} alt="brand logo" class="h-8 opacity-70 grayscale" />
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
		animation: scroll 20s linear infinite;
	}
</style>
