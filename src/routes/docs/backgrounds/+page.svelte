<script>
	import Code from '../../../components/Code.svelte';

	const colors = ['blue', 'purple', 'cyan', 'yellow', 'pink', 'green', 'red', 'grey'];

	// copy color

	const copyColor = async (color, brightness) => {
		await navigator.clipboard.writeText(`${color}-${brightness}`).then(function () {
			let paletteBox = document.querySelector(`.${'bg-' + color}-${brightness}`);
			paletteBox.innerHTML = 'Copied';

			setTimeout(() => {
				paletteBox.innerHTML = `${color}-${brightness}`;
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
				>bg-"color name"-"brightness"</span
			>
		</p>

		<div class="types">
			<p class="font-3x mgt-2 font-400">Backgrounds :</p>
			<ul class="pdl-2">
				<li class="mgt-1">> The same pattern used in <a href="/docs/colors" class="purple-500 font-600">Colors</a> , just add "bg" in front of color like : <span class="bg-purple-500 pd-1 white">bg-purple-500</span></li>
			
			</ul>
		</div>

		<!-- Pallets -->
		
	</div>
</div>

<style>
</style>

