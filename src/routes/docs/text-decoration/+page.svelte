<script>
	import Code from '../../../components/Code.svelte';
</script>

<div>
	<div class="head">
		<p class="font-4x font-500  mgb-4">Text Decoration</p>
	</div>
	<div class="text-align">
		<p class="mgt-1">
			the shorthand property class to add decoration is look like: <span class="blue-400 font-500"
				>text-"decoration line"-"decoration thickness"-"decoration style"-"decoration color"</span
			>
		</p>

		<!-- text decoration -->
		<div class="types">
			<p class="font-3x mgt-2 font-400">Decoration Line type :</p>
			<ul class="pdl-2">
				<li class="mgt-1">> overline</li>
				<li class="mgt-1">> line-through</li>
				<li class="mgt-1">> underline</li>
			</ul>

			<p class="mgt-2">so the first part of the shorthand property is one of the type above</p>
			<p class="mgt-1">
				exemple : <span class="blue-400 font-500"
					>text-overline-"decoration thickness"-"decoration style"-"decoration color"
				</span>
			</p>
		</div>
        <!-- text thickness -->
        <div class="types">
			<p class="font-3x mgt-2 font-400">Decoration Thickness:</p>
			<ul class="pdl-2">
				<li class="mgt-1">> 1x</li>
				<li class="mgt-1">> 2x</li>
				<li class="mgt-1">> until 10x</li>
				
			</ul>

			<p class="mgt-2">now the secend part of the shorthand property is the thickness of the line </p>
			<p class="mgt-1">
				exemple : <span class="blue-400 font-500"
					>text-overline-2x-"decoration style"-"decoration color"
				</span>
			</p>
		</div>
        <!-- text style -->
        <div class="types">
			<p class="font-3x mgt-2 font-400">Decoration Style:</p>
			<ul class="pdl-2">
				<li class="mgt-1">> solid</li>
				<li class="mgt-1">> double</li>
				<li class="mgt-1">> dotted</li>
				<li class="mgt-1">> dashed</li>
				<li class="mgt-1">> wavy</li>
				
			</ul>

			<p class="mgt-2">the third part of the shorthand property is the style of the line </p>
			<p class="mgt-1">
				exemple : <span class="blue-400 font-500"
					>text-overline-2x-solid-"decoration color"
				</span>
			</p>
		</div>
        <!-- text color -->
        <div class="types">
			<p class="font-3x mgt-2 font-400">Decoration Color:</p>
			<ul class="pdl-2">
				<li class="mgt-1">> to add the color, only flow the pattern "color"-"brightness" exemple : <span class="red-500">red-500</span></li>
			</ul>

			<p class="mgt-2">the final add the color to the line </p>
			<p class="mgt-1">
				exemple : <span class="blue-400 font-500"
					>text-overline-2x-solid-red-500
				</span>
			</p>
		</div>
        <!-- exemple -->
        <p class="font-3x mgt-2 mgb-2">
            Exemple :
        </p>

        <Code code='
<p class="text-overline-2x-solid-red-500">
    text exemple
</p>
        ' />

        <!-- exemple -->
        <p class="font-3x mgt-2 mgb-2">
            Result : <span class="text-line-through-2x-solid-red-500">Text</span>
        </p>

	</div>
</div>

<style>
</style>
