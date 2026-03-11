<script>
	export let icon;
	export let heading;
	export let items = [];
	export let image;
	export let imageAlt;
</script>

<div
	class="rounded-2xl p-px sm:rounded-3xl"
	style="background: radial-gradient(53.51% 100% at 53.51% 0%, rgba(250,250,255,0.3) 0%, rgba(250,250,255,0.1) 100%);"
>
	<div
		class="flex min-h-100 flex-col gap-4 rounded-2xl bg-[#0A0914] p-6 sm:min-h-125 sm:gap-6 sm:rounded-3xl sm:p-8"
	>
		<!-- ICON -->
		<img src={icon} alt="feature icon" loading="lazy" class="h-8 w-8 sm:h-10 sm:w-10" />

		<!-- HEADING -->
		<h3 class="heading">
			{heading}
		</h3>

		<!-- FEATURES -->
		<div class="space-y-2.5 sm:space-y-3">
			{#each items as item, i (i)}
				<div class="flex items-start gap-2.5 sm:gap-3">
					<img
						src="/star.svg"
						alt="star"
						loading="lazy"
						class="mt-0.5 h-3.5 w-3.5 shrink-0 sm:mt-1 sm:h-4 sm:w-4"
					/>

					<p class="feature-text">
						{item}
					</p>
				</div>
			{/each}
		</div>

		<!-- CTA -->
		<a href="#" class="learn-more"> Learn more </a>

		<!-- IMAGE -->
		<img
			src={image}
			alt={imageAlt}
			loading="lazy"
			class="mt-2 w-full rounded-lg object-cover sm:mt-4"
		/>
	</div>
</div>

<style>
	.heading {
		font-weight: 600;
		line-height: 106%;
		color: #fafaff;
		font-size: 20px;
	}

	.feature-text {
		font-weight: 500;
		line-height: 120%;
		color: #fafaff;
		opacity: 0.7;
		font-size: 16px;
	}

	.learn-more {
		font-weight: 600;
		color: #6852d6;
		font-size: 16px;
	}

	@media (min-width: 640px) {
		.heading {
			font-size: 22px;
		}

		.feature-text {
			font-size: 17px;
		}

		.learn-more {
			font-size: 17px;
		}
	}

	@media (min-width: 1024px) {
		.heading {
			font-size: 24px;
		}

		.feature-text {
			font-size: 18px;
		}

		.learn-more {
			font-size: 18px;
		}
	}
</style>
