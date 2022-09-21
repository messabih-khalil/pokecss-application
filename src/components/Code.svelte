<script>
	import 'remixicon/fonts/remixicon.css';
	import { HighlightAuto } from 'svelte-highlight';
	import github from 'svelte-highlight/styles/gruvbox-light-soft';
	// export code from components
	export let code;
	// copy the code
	const copy = () => {
		navigator.clipboard.writeText(code).then(
			function () {
				console.log('Async: Copying to clipboard was successful!');
			},
			function (err) {
				console.error('Async: Could not copy text: ', err);
			}
		);
	};
</script>

<svelte:head>
	{@html github}
</svelte:head>

<div class="code mgt-1 mgb-3 br-2x-solid-black">
	<div class="code-header bg-blue-500 pd-1 flex justify-flex-end brb-2x-solid-black">
		<!-- copy button -->
		<button
			id="copy_button"
			class="flex align-center pdl-1 pdr-1 br-2x-solid-black bg-yellow-400 font-500"
            on:click={copy}
		>
			<i class="ri-clipboard-line" />
			<span class="mgl-1"> copy </span>
		</button>
	</div>
	<div class="code-wrap bg-yellow-400">
		<HighlightAuto {code} />
	</div>
</div>

<style>
	button{
		cursor: pointer;
	}
</style>

