<script>
	import AgentPathCard from '$lib/components/AgentPathCard.svelte';

	const cards = [
		{
			icon: '/BYOB-icon.svg',
			heading: 'BYOB - Bring Your Own (Agent) Brain',
			items: [
				'Use your existing LLM orchestration',
				'Plug into CometChat’s UI, mod, notifications, and insights',
				'Modular, protocol-compatible, and fast to implement'
			],
			image: '/Ai-BYOB.png'
		},
		{
			icon: 'Build-inside-icon.svg',
			heading: 'Build Inside CometChat',
			items: [
				'Visual Agent Builder',
				'Design prompt logic, memory, retries, tool use',
				'Simulate and ship — all from a single canvas'
			],
			image: '/AI-Build Inside-CometChat.png'
		}
	];
</script>

<section class="bg-[#0A0914] py-8 text-white">
	<div class="mx-auto grid max-w-7xl gap-10 px-6 lg:grid-cols-2">
		{#each cards as card (card)}
			<AgentPathCard {...card} />
		{/each}
	</div>
</section>
