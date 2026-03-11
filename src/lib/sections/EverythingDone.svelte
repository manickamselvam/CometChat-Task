<script>
	const features = [
		'A complete frontend and system layer for AI agents. Plug in your LLM backend or build the brain with ours.',
		'CometChat is the only full stack agent platform that combines logic, UI, moderation, notifications, and insights — without glue code.',
		'Each of these is battle-tested, used and trusted in production by real companies, across real user scenarios.'
	];
</script>

<section class="bg-[#0A0914] py-10 text-white">
	<div class="mx-auto max-w-7xl px-6">
		<div class="grid items-center gap-8 lg:grid-cols-2 lg:gap-16">
			<!-- LEFT CONTENT -->
			<div class="space-y-6 sm:space-y-8 lg:space-y-10">
				<h2
					class="text-[32px] leading-[106%] font-semibold text-[#FAFAFF] sm:text-[40px] lg:text-[48px]"
				>
					Everything you'd end up
					<span class="gradient-text"> already done. </span>
				</h2>

				<div class="space-y-4 sm:space-y-5 lg:space-y-6">
					{#each features as text, i (i)}
						<div class="flex items-start gap-3 sm:gap-4">
							<img
								src="/star.svg"
								alt="Star icon"
								loading="lazy"
								class="mt-1 h-5 w-5 shrink-0 sm:h-6 sm:w-6"
							/>

							<p class="feature-text">
								{text}
							</p>
						</div>
					{/each}
				</div>
			</div>

			<!-- RIGHT IMAGE -->
			<div class="flex justify-center lg:justify-end">
				<img
					src="/EverythingDone.png"
					alt="EverythingDone"
					loading="lazy"
					class="w-full max-w-md rounded-xl object-cover sm:max-w-lg lg:max-w-xl"
				/>
			</div>
		</div>

		<!-- Divider -->
		<div class="divider mt-8"></div>
	</div>
</section>

<style>
	.gradient-text {
		background: linear-gradient(180deg, #ffffff 37.23%, #6a55d7 126.95%);
		-webkit-background-clip: text;
		background-clip: text;
		color: transparent;
		font-size: inherit;
		font-weight: 600;
		line-height: 106%;
	}

	.feature-text {
		font-size: 18px;
		line-height: 120%;
		font-weight: 500;
		letter-spacing: 0.5%;
		color: #fafaff;
		opacity: 0.74;
	}

	@media (min-width: 640px) {
		.feature-text {
			font-size: 20px;
		}
	}

	@media (min-width: 1024px) {
		.feature-text {
			font-size: 22px;
		}
	}

	.divider {
		height: 0;
		border-top: 1px solid transparent;
		border-image: linear-gradient(
				90deg,
				rgba(250, 250, 255, 0) 0%,
				rgba(250, 250, 255, 0.1) 5%,
				rgba(250, 250, 255, 0.1) 95%,
				rgba(250, 250, 255, 0) 100%
			)
			1;
	}
</style>
