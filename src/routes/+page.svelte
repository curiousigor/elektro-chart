<script>
	import Number from '../lib/Number.svelte';

	async function printPDF() {
		window.print();
	}

	let price_blok_1 = 4.41;
	let price_blok_2 = 1.08;
	let price_blok_3 = 0.23;
	let price_blok_4 = 0.02;
	let price_blok_5 = 0.0;
</script>

<div class="print">
	<div id="content" class="pb-8">
		<h1 class=" text-xl font-semibold">Cena elektrike po urah v dnevu</h1>

		<h2 class="font-medium pt-4">November, December, Januar, Februar</h2>
		<h3 class="text-sm font-medium pt-2 pb-2">Delovni dan</h3>
		<div class="grid grid-cols-24">
			{#each { length: 24 } as _, i}
				<div class="grid col-start-[{i + 1}] col-end-[{i + 2}] hour">
					{i}:00
				</div>
			{/each}
			<div class="grid col-span-6 border-l border-slate-900 border-opacity-60">
				<div class="blok blok-3">
					<Number number={price_blok_3} /><span class="value">€/kW</span>
				</div>
			</div>
			<div class="grid col-span-1 border-l border-slate-900 border-opacity-60">
				<div class="blok blok-2">
					<Number number={price_blok_2} /><span class="value">€/kW</span>
				</div>
			</div>
			<div class="grid col-span-7 border-l border-slate-900 border-opacity-60">
				<div class="blok blok-1">
					<Number number={price_blok_1} /><span class="value">€/kW</span>
				</div>
			</div>
			<div class="grid col-span-2 border-l border-slate-900 border-opacity-60">
				<div class="blok blok-2">
					<Number number={price_blok_2} /><span class="value">€/kW</span>
				</div>
			</div>
			<div class="grid col-span-4 border-l border-slate-900 border-opacity-60">
				<div class="blok blok-1">
					<Number number={price_blok_1} /><span class="value">€/kW</span>
				</div>
			</div>
			<div class="grid col-span-2 border-l border-slate-900 border-opacity-60">
				<div class="blok blok-2">
					<Number number={price_blok_2} /><span class="value">€/kW</span>
				</div>
			</div>
			<div class="grid col-span-2 border-l border-slate-900 border-opacity-60">
				<div class="blok blok-3">
					<Number number={price_blok_3} /><span class="value">€/kW</span>
				</div>
			</div>
		</div>
		<h3 class="text-sm font-medium pt-2 pb-2">Dela prost dan</h3>
		<div class="grid grid-cols-24">
			{#each { length: 24 } as _, i}
				<div class="grid col-start-[{i + 1}] col-end-[{i + 2}] hour">
					{i}:00
				</div>
			{/each}
			<div class="grid col-span-6 border-l border-slate-900 border-opacity-60">
				<div class="blok blok-4">
					<Number number={price_blok_4} /><span class="value">€/kW</span>
				</div>
			</div>
			<div class="grid col-span-1 border-l border-slate-900 border-opacity-60">
				<div class="blok blok-3">
					<Number number={price_blok_3} /><span class="value">€/kW</span>
				</div>
			</div>
			<div class="grid col-span-7 border-l border-slate-900 border-opacity-60">
				<div class="blok blok-2">
					<Number number={price_blok_2} /><span class="value">€/kW</span>
				</div>
			</div>
			<div class="grid col-span-2 border-l border-slate-900 border-opacity-60">
				<div class="blok blok-3">
					<Number number={price_blok_3} /><span class="value">€/kW</span>
				</div>
			</div>
			<div class="grid col-span-4 border-l border-slate-900 border-opacity-60">
				<div class="blok blok-2">
					<Number number={price_blok_2} /><span class="value">€/kW</span>
				</div>
			</div>
			<div class="grid col-span-2 border-l border-slate-900 border-opacity-60">
				<div class="blok blok-3">
					<Number number={price_blok_3} /><span class="value">€/kW</span>
				</div>
			</div>
			<div class="grid col-span-2 border-l border-slate-900 border-opacity-60">
				<div class="blok blok-4">
					<Number number={price_blok_4} /><span class="value">€/kW</span>
				</div>
			</div>
		</div>

		<h2 class="font-medium pt-8">Marec, April, Maj, Junij, Julij, Avgust, September, Oktober</h2>
		<h3 class="text-sm font-medium pt-2 pb-2">Delovni dan</h3>
		<div class="grid grid-cols-24">
			{#each { length: 24 } as _, i}
				<div class="grid col-start-[{i + 1}] col-end-[{i + 2}] hour">
					{i}:00
				</div>
			{/each}
			<div class="grid col-span-6 border-l border-slate-900 border-opacity-60">
				<div class="blok blok-4">
					<Number number={price_blok_4} /><span class="value">€/kW</span>
				</div>
			</div>
			<div class="grid col-span-1 border-l border-slate-900 border-opacity-60">
				<div class="blok blok-3">
					<Number number={price_blok_3} /><span class="value">€/kW</span>
				</div>
			</div>
			<div class="grid col-span-7 border-l border-slate-900 border-opacity-60">
				<div class="blok blok-2">
					<Number number={price_blok_2} /><span class="value">€/kW</span>
				</div>
			</div>
			<div class="grid col-span-2 border-l border-slate-900 border-opacity-60">
				<div class="blok blok-3">
					<Number number={price_blok_3} /><span class="value">€/kW</span>
				</div>
			</div>
			<div class="grid col-span-4 border-l border-slate-900 border-opacity-60">
				<div class="blok blok-2">
					<Number number={price_blok_2} /><span class="value">€/kW</span>
				</div>
			</div>
			<div class="grid col-span-2 border-l border-slate-900 border-opacity-60">
				<div class="blok blok-3">
					<Number number={price_blok_3} /><span class="value">€/kW</span>
				</div>
			</div>
			<div class="grid col-span-2 border-l border-slate-900 border-opacity-60">
				<div class="blok blok-4">
					<Number number={price_blok_4} /><span class="value">€/kW</span>
				</div>
			</div>
		</div>
		<h3 class="text-sm font-medium pt-2 pb-2">Dela prost dan</h3>
		<div class="grid grid-cols-24">
			{#each { length: 24 } as _, i}
				<div class="grid col-start-[{i + 1}] col-end-[{i + 2}] hour">
					{i}:00
				</div>
			{/each}
			<div class="grid col-span-6 border-l border-slate-900 border-opacity-60">
				<div class="blok blok-5">
					<Number number={price_blok_5} /><span class="value">€/kW</span>
				</div>
			</div>
			<div class="grid col-span-1 border-l border-slate-900 border-opacity-60">
				<div class="blok blok-4">
					<Number number={price_blok_4} /><span class="value">€/kW</span>
				</div>
			</div>
			<div class="grid col-span-7 border-l border-slate-900 border-opacity-60">
				<div class="blok blok-3">
					<Number number={price_blok_3} /><span class="value">€/kW</span>
				</div>
			</div>
			<div class="grid col-span-2 border-l border-slate-900 border-opacity-60">
				<div class="blok blok-4">
					<Number number={price_blok_4} /><span class="value">€/kW</span>
				</div>
			</div>
			<div class="grid col-span-4 border-l border-slate-900 border-opacity-60">
				<div class="blok blok-3">
					<Number number={price_blok_3} /><span class="value">€/kW</span>
				</div>
			</div>
			<div class="grid col-span-2 border-l border-slate-900 border-opacity-60">
				<div class="blok blok-4">
					<Number number={price_blok_4} /><span class="value">€/kW</span>
				</div>
			</div>
			<div class="grid col-span-2 border-l border-slate-900 border-opacity-60">
				<div class="blok blok-5">
					<Number number={price_blok_5} /><span class="value">€/kW</span>
				</div>
			</div>
		</div>

		<div class="flex gap-4 pt-8 col-span-full">
			<div class="flex items-center gap-1.5 text-xs">
				<div class="blok-1 h-full w-3"></div>
				<div class="flex-col items-center p-0 m-0 font-medium">
					Blok 1
					<span class="value">
						<input type="number" step=".01" bind:value={price_blok_1} class="w-10 p-0 m-0" />€/kW
					</span>
				</div>
			</div>
			<div class="flex items-center gap-1.5 text-xs">
				<div class="blok-2 h-full w-3"></div>
				<div class="flex-col items-center p-0 m-0 font-medium">
					Blok 2
					<span class="value">
						<input type="number" step=".01" bind:value={price_blok_2} class="w-10" />€/kW
					</span>
				</div>
			</div>
			<div class="flex items-center gap-1.5 text-xs">
				<div class="blok-3 h-full w-3"></div>
				<div class="flex-col items-center p-0 m-0 font-medium">
					Blok 3
					<span class="value">
						<input type="number" step=".01" bind:value={price_blok_3} class="w-10" />€/kW
					</span>
				</div>
			</div>
			<div class="flex items-center gap-1.5 text-xs">
				<div class="blok-4 h-full w-3"></div>
				<div class="flex-col items-center p-0 m-0 font-medium">
					Blok 4
					<span class="value">
						<input type="number" step=".01" bind:value={price_blok_4} class="w-10" />€/kW
					</span>
				</div>
			</div>
			<div class="flex items-center gap-1.5 text-xs">
				<div class="blok-5 h-full w-3"></div>
				<div class="flex-col items-center p-0 m-0 font-medium">
					Blok 5
					<span class="value">
						<input type="number" step=".01" bind:value={price_blok_5} class="w-10" />€/kW
					</span>
				</div>
			</div>
		</div>
	</div>
	<button on:click={printPDF} class="py-2 px-4 bg-blue-500 text-white rounded-md">Shrani PDF</button
	>
</div>

<style>
	.hour {
		@apply text-xs pb-1 border-l border-slate-900 border-opacity-60 pl-0.5 text-slate-700;
	}

	.value {
		@apply block opacity-50 font-normal text-xs;
	}

	.blok {
		@apply text-center text-sm font-semibold py-2.5;
	}

	.blok-1 {
		@apply bg-red-500;
	}

	.blok-2 {
		@apply bg-orange-400;
	}

	.blok-3 {
		@apply bg-amber-300;
	}

	.blok-4 {
		@apply bg-green-300;
	}

	.blok-5 {
		@apply bg-emerald-100;
	}

	.print {
		@apply max-w-screen-2xl mx-auto px-2 py-16;
	}

	@media print {
		@page {
			size: landscape;
		}

		button {
			display: none;
		}

		.print {
			@apply p-0;
		}
	}
</style>
