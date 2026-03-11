<script>
	const features = [
		'Resolution rates, fallback frequency, retry counts, latency',
		'Tool usage breakdowns, prompt paths, knowledge base hits',
		'Conversation-level analytics: drop-off points, re-engagement, success outcomes',
		'Sentiment markers and feedback loops',
		'Exportable, filterable, and privacy-respectful'
	];
</script>

<section class="bg-[#0A0914] py-10 text-white">
	<div class="mx-auto max-w-7xl px-6">
		<div class="grid grid-cols-1 items-center gap-8 lg:grid-cols-2 lg:gap-16">
			<!-- LEFT CONTENT -->
			<div class="space-y-6 sm:space-y-8">
				<a
					href="#"
					class="inline-block text-[18px] leading-[106%] font-semibold text-[#6852D6] sm:text-[20px] lg:text-[22px]"
				>
					Insights dashboard
				</a>

				<h2
					class="text-[28px] leading-[106%] font-semibold text-[#FAFAFF] sm:text-[32px] lg:text-[36px]"
				>
					Ship the agent. Then make it better. Without needing Mixpanel, Segment, or BI setups.
				</h2>

				<p class="feature-text">
					From day one, you get built-in visibility into what your agent is doing — and how people
					are responding.
				</p>

				<!-- FEATURE LIST -->
				<div class="space-y-3 sm:space-y-4">
					{#each features as feature, i (i)}
						<div class="flex items-start gap-3 sm:gap-4">
							<img
								src="/star.svg"
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

				<p class="feature-text">
					You can't improve what you can't see. With us, you never ship blind.
				</p>
			</div>

			<!-- RIGHT IMAGE -->
			<div class="flex justify-center lg:justify-end">
				<img
					src="/insight-dashboard.png"
					alt="Insight Dashboard"
					loading="lazy"
					class="w-full max-w-md rounded-xl object-cover sm:max-w-lg lg:max-w-xl"
				/>
			</div>
		</div>
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
</style>
