<script lang="ts">
	import './base.css';
	import Icon from '@iconify/svelte';

	interface Feature {
		icon: string;
		title: string;
		description: string;
	}

	export let title: string;
	export let subtitle: string;
	export let description: string;
	export let features: Feature[];
</script>

<div class="bg-white">
	<div class="mx-auto max-w-md px-4 text-center sm:max-w-3xl sm:px-6 lg:max-w-7xl lg:px-8">
		<h2 class="text-base font-semibold uppercase tracking-wider text-indigo-600">
			{subtitle}
		</h2>
		<p class="mt-2 text-3xl font-extrabold tracking-tight text-gray-900 sm:text-4xl">
			{title}
		</p>
		<p class="mx-auto mt-5 max-w-prose text-xl text-gray-500">
			{description}
		</p>
		<div class="mt-12">
			<div class="grid grid-cols-1 gap-8 sm:grid-cols-2 lg:grid-cols-3">
				{#each features as feature}
					<div class="pt-6">
						<div class="flow-root rounded-lg bg-gray-50 px-6 pb-8">
							<div class="-mt-6">
								<div>
									<span
										class="inline-flex items-center justify-center rounded-md bg-indigo-500 p-3 shadow-lg"
									>
										<Icon icon={feature.icon} class="h-6 w-6 text-white" />
									</span>
								</div>
								<h3 class="mt-8 text-lg font-medium tracking-tight text-gray-900">
									{feature.title}
								</h3>
								<p class="mt-5 text-base text-gray-500">
									{feature.description}
								</p>
							</div>
						</div>
					</div>
				{/each}
			</div>
		</div>
	</div>
</div>
