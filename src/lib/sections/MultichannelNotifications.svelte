<script>
	const features = [
		"Native push, email, and SMS support",
		"Retry logic, delivery throttling, and batching",
		"Trigger-based delivery rules — unread X mins, fallback triggered, user went silent",
		"Threaded email replies (yes, replies go back to chat!)",
		"Integrates with SendGrid, Twilio, or your custom providers",
		"User-level frequency + preference settings"
	];
</script>

<section class="bg-[#0A0914] py-8 text-white">
	<div class="mx-auto max-w-7xl px-6">

		<div class="grid items-center gap-8 lg:grid-cols-2 lg:gap-16">

			<!-- LEFT CONTENT -->
			<div class="space-y-6 sm:space-y-8">

				<a
					href="#"
					class="inline-block text-[18px] font-semibold leading-[106%] text-[#6852D6] sm:text-[20px] lg:text-[22px]"
				>
					Multichannel notifications engine
				</a>

				<h2
					class="text-[28px] font-semibold leading-[106%] text-[#FAFAFF] sm:text-[32px] lg:text-[36px]"
				>
					Your agent is only helpful if people come back to talk to it.
				</h2>

				<p class="feature-text">
					Most agents get ghosted. Yours won't.
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

				<p class="feature-text pt-3 sm:pt-4">
					Notifications aren't a growth hack. They're UX glue. And we built them so you wouldn't have
					to.
				</p>

			</div>

			<!-- RIGHT IMAGE -->
			<div class="flex justify-center lg:justify-end">
				<img
					src="/multi-channel-notification.png"
					alt="Multichannel notification"
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
			rgba(250,250,255,0) 0%,
			rgba(250,250,255,0.1) 5%,
			rgba(250,250,255,0.1) 95%,
			rgba(250,250,255,0) 100%
		) 1;
	}
</style>