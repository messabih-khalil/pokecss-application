<script>
	import Code from '../../../components/Code.svelte';
</script>

<div>
	<div class="head">
		<p class="font-4x font-500  mgb-4">Font Weight</p>
	</div>
	<div class="text-align">
		<p class="mgt-1">
			the shorthand property of font Weight : <span class="blue-400 font-500">font-"weight"</span>
		</p>

		<!-- text decoration -->
		<div class="types">
			<p class="font-3x mgt-2 font-400">Weightes :</p>
			<ul class="pdl-2">
				<li class="mgt-1">> 100 , 200 , 300 , 400 , 500 , 600 , 700 , 800 , 900</li>
			</ul>
		</div>
		<!-- exemples -->
		<div>
			<p class="font-3x mgt-2 mgb-1">Exemples :</p>
			<Code
				code='
<p class="font-100">
    Lorem ipsum dolor
</p>
<p class="font-900">
    Lorem ipsum dolor
</p>
<p class="font-800">
    Lorem ipsum dolor
</p>
<p class="font-700">
    Lorem ipsum dolor
</p>
<p class="font-600">
    Lorem ipsum dolor
</p>
<p class="font-500">
    Lorem ipsum dolor
</p>
<p class="font-400">
    Lorem ipsum dolor
</p>
<p class="font-300">
    Lorem ipsum dolor
</p>
<p class="font-200">
    Lorem ipsum dolor
</p>
<p class="font-100">
    Lorem ipsum dolor
</p>

                    '
			/>

			<!-- exemple -->
			<p class="font-3x mgt-2 mgb-2">Result : </p>
			<div>
				<p class="font-900">Lorem ipsum dolor</p>
				<p class="font-800">Lorem ipsum dolor</p>
				<p class="font-700">Lorem ipsum dolor</p>
				<p class="font-600">Lorem ipsum dolor</p>
				<p class="font-500">Lorem ipsum dolor</p>
				<p class="font-400">Lorem ipsum dolor</p>
				<p class="font-300">Lorem ipsum dolor</p>
				<p class="font-200">Lorem ipsum dolor</p>
				<p class="font-100">Lorem ipsum dolor</p>
			</div>
		</div>
	</div>
</div>

<style>
</style>
