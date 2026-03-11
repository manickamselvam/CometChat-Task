<script>
	const features = [
		"Token streaming with dynamic 'thinking…' states",
		'Retry/stop buttons with full control logic',
		'Memory pills, prompt banners, and agent selectors',
		'Structured tool replies with inline citations',
		'Slash commands, modals, and frontend triggers',
		'Low/No-code Chat Builder, or more control via UI Kits and SDKs',
		'Fully AG-UI protocol compatible — including tool call rendering, memory markers, and fallback patterns'
	];
</script>

<section class="bg-[#0A0914] py-10 text-white">
	<div class="mx-auto max-w-7xl px-6">
		<div class="grid items-center gap-8 lg:grid-cols-2 lg:gap-16">
			<!-- LEFT CONTENT -->
			<div class="space-y-6 sm:space-y-8">
				<!-- LINK -->
				<a
					href="#"
					class="inline-block text-[18px] leading-[106%] font-semibold text-[#6852D6] sm:text-[20px] lg:text-[22px]"
				>
					Production-ready chat UI
				</a>

				<!-- HEADING -->
				<h2
					class="text-[28px] leading-[106%] font-semibold text-[#FAFAFF] sm:text-[32px] lg:text-[36px]"
				>
					The UX layer your agent deserves. Built for LLM-native interactions, out of the box.
				</h2>

				<!-- DESCRIPTION -->
				<p class="feature-text">
					Forget cobbling together buttons and hoping users 'get it'. Our chat layer is
					purpose-built for how agents think — and how humans expect them to respond.
				</p>

				<!-- FEATURES -->
				<div class="space-y-3 sm:space-y-4">
					{#each features as feature, i (i)}
						<div class="flex items-start gap-3 sm:gap-4">
							<img
								src="star.svg"
								alt="star"
								loading="lazy"
								class="mt-1 h-4 w-4 shrink-0 sm:h-5 sm:w-5"
							/>

							<p class="feature-text">
								{feature}
							</p>
						</div>
					{/each}
				</div>

				<!-- FINAL NOTE -->
				<p class="feature-text">
					It's not just a pretty shell. It's UX that teaches trust, guides behavior, and makes your
					agent feel alive.
				</p>
			</div>

			<!-- RIGHT IMAGE -->
			<div class="flex justify-center lg:justify-end">
				<img
					src="production-ready-chat-ui.png"
					alt="Production ready chat interface"
					loading="lazy"
					class="w-full max-w-md rounded-xl object-cover sm:max-w-lg lg:max-w-xl"
				/>
			</div>
		</div>

		<!-- DIVIDER -->
		<div class="divider mt-12 sm:mt-16 lg:mt-17.5"></div>
	</div>
</section>

<style>
	.feature-text {
		font-size: 16px;
		line-height: 120%;
		font-weight: 500;
		letter-spacing: 0.5%;
		color: #fafaff;
		opacity: 0.74;
	}

	@media (min-width: 640px) {
		.feature-text {
			font-size: 17px;
		}
	}

	@media (min-width: 1024px) {
		.feature-text {
			font-size: 18px;
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
