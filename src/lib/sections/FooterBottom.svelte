<script>
	const socialLinks = [
		{
			name: 'Facebook',
			icon: '/social-media/facebook.svg',
			href: '#'
		},
		{
			name: 'LinkedIn',
			icon: '/social-media/linkedin.svg',
			href: '#'
		},
		{
			name: 'Instagram',
			icon: '/social-media/Instagram.svg',
			href: '#'
		},
		{
			name: 'Twitter',
			icon: '/social-media/twitter.svg',
			href: '#'
		},
		{
			name: 'GitHub',
			icon: '/social-media/github.svg',
			href: '#'
		}
	];

	const TEXT_CLASS =
		"font-['Satoshi_Variable'] text-[13px] leading-[140%] font-semibold tracking-[2%] text-[#FAFAFF] opacity-74 sm:text-[14px]";
</script>

<footer class="bg-[#0A0914] text-white">
	<div class="mx-auto max-w-7xl px-4 py-6 sm:px-6 sm:py-8 lg:px-0">
		<!-- Logo -->
		<div class="mb-6 sm:mb-8">
			<img
				src="/CometChat-Logo-footer-transparent.png"
				alt="CometChat Logo"
				class="mx-auto h-auto w-full sm:mx-0"
			/>
		</div>

		<hr
			class="mb-6 opacity-100 sm:mb-8"
			style="border-image: linear-gradient(90deg, rgba(39, 39, 48, 0) 0%, #272730 47.92%, rgba(39, 39, 48, 0) 100%) 1;"
		/>

		<!-- Bottom Bar -->
		<div class="flex flex-col items-start justify-between gap-6 md:flex-row md:gap-4">
			<!-- Social Links -->
			<div class="flex flex-wrap items-center gap-4 sm:gap-5 md:order-2 md:gap-6">
				{#each socialLinks as social (social.name)}
					<a
						href={social.href}
						class="flex items-center gap-1.5 text-sm text-gray-400 transition-colors hover:text-white sm:gap-2"
					>
						<img src={social.icon} alt={social.name} class="h-4 w-4" />

						<span class={TEXT_CLASS}>
							{social.name}
						</span>
					</a>
				{/each}
			</div>

			<!-- Copyright -->
			<div class="flex flex-wrap items-center gap-3 text-sm text-gray-400 sm:gap-4 md:order-1">
				<span class={TEXT_CLASS}>2025 © CometChat</span>

				<a href="#" class={`${TEXT_CLASS} hover:opacity-100`}> Terms of Use </a>

				<a href="#" class={`${TEXT_CLASS} hover:opacity-100`}> Privacy Policy </a>
			</div>
		</div>
	</div>
</footer>
