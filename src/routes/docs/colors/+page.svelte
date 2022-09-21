<script>
	import Code from '../../../components/Code.svelte';

	const colors = ['blue', 'purple', 'cyan', 'yellow', 'pink', 'green', 'red', 'grey'];

	// copy color

	const copyColor = async (color, brightness) => {
		await navigator.clipboard.writeText(`${color}-${brightness}`).then(function () {
			let paletteBox = document.querySelector(`.${'bg-' + color}-${brightness}`);
			paletteBox.innerHTML = 'Copied';

			setTimeout(() => {
				paletteBox.innerHTML = `${brightness}`;
			}, 1000);
		});
	};

	let counter = 0;
</script>

<div>
	<div class="head">
		<p class="font-4x font-500  mgb-4">Colors</p>
	</div>
	<div class="text-align">
		<p class="mgt-1">
			the shorthand property of color : <span class="blue-400 font-500"
				>"color name"-"brightness"</span
			>
		</p>

		<div class="types">
			<p class="font-3x mgt-2 font-400">Colors names :</p>
			<ul class="pdl-2">
				<li class="mgt-1">> Blue</li>
				<li class="mgt-1">> Red</li>
				<li class="mgt-1">> Purple</li>
				<li class="mgt-1">> cyan</li>
				<li class="mgt-1">> yellow</li>
				<li class="mgt-1">> Pink</li>
				<li class="mgt-1">> Green</li>
				<li class="mgt-1">> Grey</li>
			</ul>
		</div>

		<div class="types">
			<p class="font-3x mgt-2 font-400">Brightness :</p>
			<ul class="pdl-2">
				<li class="mgt-1">> From 50 to 900</li>
			</ul>
		</div>
		<!-- Pallets -->
		<div>
			<p class="font-3x mgt-2 mgb-1">Palettes :</p>
			<p class="green-800 flex align-center font-3x">
				<i class="ri-information-fill font-4x mgr-1"></i>
				<span>
					Click in any palette to copy color
				</span>

			</p>

			{#each colors as color}
				<p class="font-2x mgt-2 mgb-1 font-500 {color}-400">{color} :</p>
				<!-- palette boxes -->
				<div class="grid-xl-8 grid-lg-6 grid-md-4 grid-sm-3 grid-xs-2 gap-2">
					<div
						class="color-box bg-{color}-50 flex align-center justify-center"
						on:click={() => copyColor({ color }, '50')}
					>
						50
					</div>
					{#each Array(9) as key, i}
						<!-- box -->
						<div
							class="color-box bg-{color}-{(i + 1) * 100} flex align-center justify-center"
							on:click={() => copyColor(color, (i + 1) * 100)}
						>
							{(i + 1) * 100}
						</div>
					{/each}
					{#if color != 'grey'}
						{#each Array(4) as _, i}
							<!-- box -->
							<div
								class="color-box bg-{color}-a{(i + 1) * 100} flex align-center justify-center"
								on:click={() => copyColor(color, 'a' + (i + 1) * 100)}
							>
								a{(i + 1) * 100}
							</div>
						{/each}
					{/if}
				</div>
			{/each}
		</div>
	</div>
</div>

<style>
	.color-box {
		height: 100px;
		width: 100px;
		cursor: pointer;
	}
</style>
