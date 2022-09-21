<script>
	import Code from '../../../components/Code.svelte';
</script>

<div>
	<div class="head">
		<p class="font-4x font-500  mgb-4">Font Size</p>
	</div>
	<div class="text-align">
		<p class="mgt-1">
			the shorthand size property : <span class="blue-400 font-500">font-"size from 1 to 10"x</span>
		</p>

		<!-- text decoration -->
		<div class="types">
			<p class="font-3x mgt-2 font-400">Sizes :</p>
			<ul class="pdl-2">
				<li class="mgt-1">> 1x , 2x , 3x , 4x , 5x , 6x , 7x , 8x , 9x , 10x</li>
			</ul>
		</div>
		<!-- exemples -->
		<div>
			<p class="font-3x mgt-2 mgb-1">Exemples :</p>
			<Code
				code='
<p class="font-10x">
    Lorem ipsum dolor
</p>
<p class="font-9x">
    Lorem ipsum dolor
</p>
<p class="font-8x">
    Lorem ipsum dolor
</p>
<p class="font-7x">
    Lorem ipsum dolor
</p>
<p class="font-6x">
    Lorem ipsum dolor
</p>
<p class="font-5x">
    Lorem ipsum dolor
</p>
<p class="font-4x">
    Lorem ipsum dolor
</p>
<p class="font-3x">
    Lorem ipsum dolor
</p>
<p class="font-2x">
    Lorem ipsum dolor
</p>
<p class="font-1x">
    Lorem ipsum dolor
</p>

                    '
			/>

			<!-- exemple -->
			<p class="font-3x mgt-2 mgb-2">Result : </p>
			<div>
				<p class="font-10x">Lorem ipsum dolor</p>
				<p class="font-9x">Lorem ipsum dolor</p>
				<p class="font-8x">Lorem ipsum dolor</p>
				<p class="font-7x">Lorem ipsum dolor</p>
				<p class="font-6x">Lorem ipsum dolor</p>
				<p class="font-5x">Lorem ipsum dolor</p>
				<p class="font-4x">Lorem ipsum dolor</p>
				<p class="font-3x">Lorem ipsum dolor</p>
				<p class="font-2x">Lorem ipsum dolor</p>
				<p class="font-1x">Lorem ipsum dolor</p>
			</div>
		</div>
	</div>
</div>

<style>
</style>
