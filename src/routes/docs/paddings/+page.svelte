<script>
	import Code from '../../../components/Code.svelte';
</script>

<div>
	<div class="head">
		<p class="font-4x font-500  mgb-4">Paddings</p>
	</div>
	<div class="text-align">
		<p class="mgt-1">
			the shorthand property of padding : <span class="blue-400 font-500">pd"the side"-"size"</span>
		</p>

		<div class="types">
			<p class="font-3x mgt-2 font-400">Padding names :</p>
			<ul class="pdl-2">
				<li class="mgt-1">> pd : global padding</li>
				<li class="mgt-1">> pdt : padding-top</li>
				<li class="mgt-1">> pdb : padding-bottom</li>
				<li class="mgt-1">> pdl : padding-left</li>
				<li class="mgt-1">> pdr : padding-right</li>
			</ul>
		</div>

		<div class="types">
			<p class="font-3x mgt-2 font-400">Padding size :</p>
			<ul class="pdl-2">
				<li class="mgt-1">> From 1 to 10</li>
			</ul>
		</div>

		<!-- exemples -->

		<div class="exemples">
			<p class="font-3x mgt-2">
				Exemples : <span class="blue-400">pd-2</span>
			</p>
			<!-- code -->
			<Code
				code='
<div class="pd-2">
    <p class="bg-yellow-400 pd-2">
        this is global padding
    </p>
</div>
            '
			/>

			<p class="font-3x mgt-2">Result :</p>

			<div class="pd-2 bg-green-400 mgt-2">
				<p class="bg-yellow-400 pd-2">this is global padding</p>
			</div>
		</div>
		<div class="exemples">
			<p class="font-3x mgt-2">
				Exemples : <span class="blue-400">pdt-2</span>
			</p>
			<!-- code -->
			<Code
				code='
<div class="pdt-2">
    <p class="bg-yellow-400 pdt-2">
        this is top padding
    </p>
</div>
            '
			/>

			<p class="font-3x mgt-2">Result :</p>

			<div class="pdt-2 bg-green-400 mgt-2">
				<p class="bg-yellow-400 pdt-2">this is top padding</p>
			</div>
		</div>
		<div class="exemples">
			<p class="font-3x mgt-2">
				Exemples : <span class="blue-400">pdb-2</span>
			</p>
			<!-- code -->
			<Code
				code='
<div class="pdb-2">
    <p class="bg-yellow-400 pdb-2">
        this is bottom padding
    </p>
</div>
            '
			/>

			<p class="font-3x mgt-2">Result :</p>

			<div class="pdb-2 bg-green-400 mgt-2">
				<p class="bg-yellow-400 pdb-2">this is bottom padding</p>
			</div>
		</div>
		<div class="exemples">
			<p class="font-3x mgt-2">
				Exemples : <span class="blue-400">pdl-2</span>
			</p>
			<!-- code -->
			<Code
				code='
<div class="pdl-2">
    <p class="bg-yellow-400 pdl-2">
        this is left padding
    </p>
</div>
            '
			/>

			<p class="font-3x mgt-2">Result :</p>

			<div class="pdl-2 bg-green-400 mgt-2">
				<p class="bg-yellow-400 pdl-2">this is global padding</p>
			</div>
		</div>
		<div class="exemples">
			<p class="font-3x mgt-2">
				Exemples : <span class="blue-400">pdr-2</span>
			</p>
			<!-- code -->
			<Code
				code='
<div class="pdr-2">
    <p class="bg-yellow-400 pdr-2">
        this is right padding
    </p>
</div>
            '
			/>

			<p class="font-3x mgt-2">Result :</p>

			<div class="pdr-2 bg-green-400 mgt-2">
				<p class="bg-yellow-400 pdr-2">this is right padding</p>
			</div>
		</div>
	</div>
</div>

<style>
	
</style>
