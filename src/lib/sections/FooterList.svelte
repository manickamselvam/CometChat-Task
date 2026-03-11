<script>
	const footerSections = [
		{
			column: 'Platform',
			groups: [
				{
					title: 'Platform',
					links: [
						{ text: 'Chat & Messaging', href: '#' },
						{ text: 'Voice & Video Calls', href: '#' }
					]
				},
				{
					title: 'Features',
					links: [
						{ text: 'Chat & Messaging', href: '#' },
						{ text: 'Voice & Video Calls', href: '#' },
						{ text: 'Notifications', href: '#' },
						{ text: 'Analytics & Insights', href: '#' },
						{ text: 'Multi-Tenant Chat', href: '#' }
					]
				},
				{
					title: 'Integration Methods',
					links: [
						{ text: 'UI Kits', href: '#' },
						{ text: 'SDKs & APIs', href: '#' }
					]
				}
			]
		},
		{
			column: 'Solutions',
			groups: [
				{
					title: 'Solutions',
					links: [
						{ text: 'By Use cases', href: '#' },
						{ text: 'On-demand', href: '#' },
						{ text: 'Online Marketplaces', href: '#' },
						{ text: 'SaaS Businesses', href: '#' },
						{ text: 'Healthcare & Telehealth', href: '#' },
						{ text: 'Community & Social', href: '#' },
						{ text: 'Dating', href: '#' }
					]
				},
				{
					title: 'Comparison',
					links: [
						{ text: 'CometChat vs Sendbird', href: '#' },
						{ text: 'Compare Top Chat SDKs', href: '#' },
						{ text: 'Sendbird Alternatives', href: '#' },
						{ text: 'Stream Chat Alternatives', href: '#' }
					]
				}
			]
		},
		{
			column: 'Developers',
			groups: [
				{
					title: 'Developers',
					links: [
						{ text: 'Docs', href: '#' },
						{ text: 'Sample Apps', href: '#' },
						{ text: 'APIs', href: '#' },
						{ text: 'Product Updates', href: '#' },
						{ text: 'Feature Requests', href: '#' },
						{ text: 'System Status', href: '#' }
					]
				},
				{
					title: 'Support',
					links: [
						{ text: 'Community', href: '#' },
						{ text: 'Help Center', href: '#' },
						{ text: 'Office Hours', href: '#' },
						{ text: 'Report an issue', href: '#' }
					]
				}
			]
		},
		{
			column: 'Resources',
			groups: [
				{
					title: 'Resources',
					links: [
						{ text: 'Templates', href: '#' },
						{ text: 'Tutorials', href: '#' },
						{ text: 'Blog', href: '#' }
					]
				},
				{
					title: 'Chat UI Kits',
					links: [
						{ text: 'React Chat UI Kit', href: '#' },
						{ text: 'Flutter Chat UI Kit', href: '#' },
						{ text: 'Android Chat UI Kit', href: '#' },
						{ text: 'React Native Chat UI Kit', href: '#' },
						{ text: 'iOS Chat UI Kit', href: '#' }
					]
				}
			]
		},
		{
			column: 'Company',
			groups: [
				{
					title: 'Company',
					links: [
						{ text: 'Careers', href: '#' },
						{ text: 'Partners', href: '#' },
						{ text: 'Pricing', href: '#' },
						{ text: 'Implementation Services', href: '#' },
						{ text: 'Chat with us', href: '#' }
					]
				},
				{
					title: 'Terms and Legal',
					links: [
						{ text: 'Terms of Service', href: '#' },
						{ text: 'Privacy Policy', href: '#' },
						{ text: 'Sub-processors List', href: '#' },
						{ text: 'Data Processing Addendum', href: '#' },
						{ text: 'Vulnerability Disclosure Program', href: '#' }
					]
				}
			]
		}
	];

	// Define which titles should be blue (main column titles)
	const blueHeaders = ['Platform', 'Solutions', 'Developers', 'Resources', 'Company'];

	// Track open sections for mobile accordion
	let openSections = {};

	// Function to toggle accordion
	function toggleSection(columnName) {
		openSections[columnName] = !openSections[columnName];
	}

	// Function to get header color class
	function getHeaderColor(title) {
		return blueHeaders.includes(title)
			? `font-['Satoshi_Variable'] font-semibold text-[16px] leading-[112%] tracking-[0.5%] text-[#6852D6]`
			: `opacity-54 font-['Satoshi_Variable'] font-semibold text-[14px] leading-[140%] tracking-[2%] text-[#FAFAFF]`;
	}
</script>

<footer class="bg-[#0A0914] px-6 py-12 text-white sm:px-8 sm:py-16">
	<div class="mx-auto max-w-7xl">
		<!-- Logo -->
		<div class="mb-8 sm:mb-12">
			<img src="/Logo.svg" alt="cometchat logo" class="h-7 sm:h-8" />
		</div>

		<!-- Mobile Accordion View (< lg) -->
		<div class="space-y-4 lg:hidden">
			{#each footerSections as section (section.column)}
				<div>
					<!-- Accordion Header -->
					<button
						on:click={() => toggleSection(section.column)}
						class="flex w-full items-center justify-between py-4 text-left"
					>
						<h3 class="font-['Satoshi_Variable'] text-[18px] font-semibold leading-[112%] tracking-[0.5%] text-[#6852D6]">
							{section.column}
						</h3>
						<span class="text-[24px] text-[#6852D6] transition-transform duration-200" class:rotate-45={openSections[section.column]}>
							+
						</span>
					</button>

					<!-- Accordion Content -->
					{#if openSections[section.column]}
						<div class="pb-4 transition-all duration-300">
							{#each section.groups as group (group.title)}
								<div class:mt-6={group !== section.groups[0]}>
									{#if !blueHeaders.includes(group.title)}
										<h4 class="mb-3 {getHeaderColor(group.title)}">
											{group.title}
										</h4>
									{/if}
									<ul class="space-y-2.5">
										{#each group.links as link (`${group.title}-${link.text}`)}
											<li>
												<a
													href={link.href}
													class="opacity-84 font-['Satoshi_Variable'] text-[14px] font-semibold leading-[140%] tracking-[2%] text-[#FAFAFF]"
												>
													{link.text}
												</a>
											</li>
										{/each}
									</ul>
								</div>
							{/each}
						</div>
					{/if}
				</div>
			{/each}
		</div>

		<!-- Desktop Grid View (>= lg) -->
		<div class="hidden grid-cols-2 gap-8 md:grid-cols-3 lg:grid lg:grid-cols-5 lg:gap-12">
			{#each footerSections as section (section.column)}
				<div>
					{#each section.groups as group (group.title)}
						<div class:mt-8={group !== section.groups[0]}>
							<h3 class="mb-4 {getHeaderColor(group.title)}">
								{group.title}
							</h3>
							<ul class="space-y-3">
								{#each group.links as link (`${group.title}-${link.text}`)}
									<li>
										<a
											href={link.href}
											class="opacity-84 font-['Satoshi_Variable'] text-[14px] font-semibold leading-[140%] tracking-[2%] text-[#FAFAFF]"
										>
											{link.text}
										</a>
									</li>
								{/each}
							</ul>
						</div>
					{/each}
				</div>
			{/each}
		</div>
	</div>
</footer>