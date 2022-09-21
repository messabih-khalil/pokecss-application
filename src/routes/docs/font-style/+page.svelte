<script>
	import Code from '../../../components/Code.svelte';
</script>

<div>
	<div class="head">
		<p class="font-4x font-500  mgb-4">Font Weight</p>
	</div>
	<div class="text-align">
		<p class="mgt-1">
			the shorthand property of font style : <span class="blue-400 font-500">font-"style"</span>
		</p>

		<!-- text decoration -->
		<div class="types">
			<p class="font-3x mgt-2 font-400">Styles :</p>
			<ul class="pdl-2">
				<li class="mgt-1">> normal - The text is shown normally</li>
				<li class="mgt-1">> italic - The text is shown in italics</li>
				<li class="mgt-1">> oblique - The text is "leaning" (oblique is very similar to italic, but less supported)
                </li>
			</ul>
		</div>
		<!-- exemples -->
		<div>
			<p class="font-3x mgt-2 mgb-1">Exemples :</p>
			<Code
				code='
<p class="font-normal">
    Lorem ipsum dolor
</p>
<p class="font-italic">
    Lorem ipsum dolor
</p>
<p class="font-oblique">
    Lorem ipsum dolor
</p>
                    '
			/>

			<!-- exemple -->
			<p class="font-3x mgt-2 mgb-2">Result : </p>
			<div>
				<p class="font-normal mgt-1">
                    Lorem ipsum dolor
                </p>
                <p class="font-italic mgt-1">
                    Lorem ipsum dolor
                </p>
                <p class="font-oblique mgt-1">
                    Lorem ipsum dolor
                </p>
			</div>
		</div>
	</div>
</div>

<style>
</style>
