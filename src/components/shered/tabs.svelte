<script>
	import { createEventDispatcher } from 'svelte';
	const dispatch = createEventDispatcher();
	export let items;
	export let activeItem;
</script>

<div class="bg-gray-100 border-b-2  shadow-sm text-center p-10 sm:w-full">
	<div class="w-5/12 m-auto">
		<ul class="flex justify-between">
			{#each items as item}
				<li on:click={() => dispatch('tabChange', item)}>
					<div
						class="text-orange-400 border-b-2 cursor-pointer font-bold text-2xl hover:text-orange-600 duration-300 transition-all hover:border-orange-600 p-2 "
						class:active={item === activeItem}
					>
						{item}
					</div>
				</li>
			{/each}
		</ul>
	</div>
</div>

<style>
	.active {
		color: #ea580c;
	}
</style>
