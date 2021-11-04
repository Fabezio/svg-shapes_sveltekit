<script context="module" lang="ts">
	export const prerender = true;
</script>

<script lang="ts">
	import SVG1 from '$lib/SVG1.svelte';
	import SVG2 from '$lib/SVG2.svelte';
	import SVG3 from '$lib/SVG3.svelte';
	import SVG4 from '$lib/SVG4.svelte';
	import SVG0 from '$lib/SVG0.svelte';

	const title = 'Carrés';
	let number = 0;
	let slots = [];
	let rest = number % 5;
	const options = [
		{ component: SVG0 },
		{ component: SVG1 },
		{ component: SVG2 },
		{ component: SVG3 },
		{ component: SVG4 }
	];
	let selected = options[rest];
	function handleRest(e) {
		rest = number % 5;
		if (rest === 0) slots = [...slots, { component: SVG0 }];

		selected = options[rest];
	}

	$: console.log(slots.length);
</script>

<svelte:head>
	<title>{title}</title>
</svelte:head>
<h1>{title}</h1>

<section>
	<h2>
		{slots.length} - {rest}
	</h2>

	<input type="number" on:change={handleRest} bind:value={number} />
	<div
		class="container"
		style="grid-template-columns: repeat({slots.length}, 1fr){rest > 0 ? ' 1fr' : ''} ;"
	>
		{#if number > 0}
			{#each slots as slot}
				<SVG0 />
			{/each}

			{#if rest > 0}
				<svelte:component this={selected.component} />
			{/if}
		{/if}
	</div>
</section>

<style>
	.container {
		min-height: 100px;
		min-width: 50px;
		display: grid;
		grid-gap: 1em;
	}
	section {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		flex: 1;
	}

	h1 {
		width: 100%;
	}
</style>
