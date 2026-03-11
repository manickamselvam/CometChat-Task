<script>
	import { onMount } from 'svelte';
	
	let isMobile = false;

	onMount(() => {
		const checkMobile = () => {
			isMobile = window.innerWidth < 768; // 768px is the 'md' breakpoint
		};
		
		checkMobile();
		window.addEventListener('resize', checkMobile);
		
		return () => window.removeEventListener('resize', checkMobile);
	});
</script>

<div class="bg-[#0A0914] pt-6 sm:pt-8 lg:pt-10">
	<div class="relative mx-auto max-w-6xl px-0 sm:px-4">
		<img 
			src={isMobile ? "/Planat-of-cometchat-mobile.png" : "/Planat-of-cometchat.png"} 
			alt="cometchat icon" 
			class="mx-auto w-full" 
		/>

		<!-- Text Content inside ARC -->
		<div
			class="absolute bottom-38 left-1/2 flex w-full -translate-x-1/2 flex-col items-center px-4 text-center sm:bottom-3 sm:px-6 lg:bottom-4 lg:w-[58%] lg:px-8"
		>
			<h1 class="max-w-full text-[24px] leading-[106%] font-semibold text-[#FAFAFF] sm:text-[32px] md:text-[40px] lg:text-[48px]">
				You don't need to build it <br class="hidden sm:block" /> all to ship it all
			</h1>

			<p class="mt-2 max-w-full text-[14px] leading-[120%] font-medium text-[#FAFAFF] opacity-70 sm:mt-3 sm:text-[16px] md:text-[18px] lg:mt-4 lg:text-[22px]">
				Start with chat. Or go full stack. Build fast, scale securely, and focus on what your agent
				does - not what it's missing.
			</p>

			<div class="mt-3 flex flex-wrap justify-center gap-2 sm:mt-4 sm:gap-3 lg:mt-6 lg:gap-4">
				<button
					class="flex h-9 cursor-pointer items-center gap-2 rounded-lg border border-[#FAFAFF1A] px-3 py-2 sm:h-10 sm:gap-2.5 sm:rounded-xl sm:px-4 sm:py-2.5 lg:h-11 lg:py-3"
				>
					<span class="text-[12px] font-semibold text-[#FAFAFF] sm:text-[13px] lg:text-[14px]">Talk to Us</span>
				</button>

				<button
					class="flex h-9 cursor-pointer items-center justify-center gap-2 rounded-lg bg-[#6852D6] px-3 py-2 sm:h-10 sm:gap-2.5 sm:rounded-xl sm:px-4 sm:py-2.5 lg:h-11 lg:py-3"
				>
					<span class="text-[12px] font-semibold text-[#FAFAFF] sm:text-[13px] lg:text-[14px]"> Try the Agent Builder </span>
				</button>
			</div>
		</div>
	</div>
</div>