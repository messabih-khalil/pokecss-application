<script>
	import { pandaSyntaxDark } from 'svelte-highlight/styles';
	import Code from '../../../components/Code.svelte';
</script>

<div>
	<div class="head">
		<p class="font-4x font-500  mgb-4">Display</p>
	</div>
	<div class="text-align">
		<p class="mgt-1">
			the shorthand property of margin : <span class="blue-400 font-500">"typ of display"</span>
		</p>

		<div class="types">
			<p class="font-3x mgt-2 font-400">Display types :</p>
			<ul class="pdl-2">
				<li class="mgt-1">> block => display : block;</li>
				<li class="mgt-1">> none => display : none;</li>
				<li class="mgt-1">> flex => display : flex;</li>
				<li class="mgt-1">> grid => display : grid;</li>
				<li class="mgt-1">> inline => display : inline;</li>
				<li class="mgt-1">> inline-block => display : inline-block;</li>
                <li class="mgt-1 blue-a200 font-3x font-500">Usage : class="type of display"  , exp : class="block"  </li>
			</ul>
		</div>
		<!-- exemple -->
		<div>
			<p class="font-3x mgt-2 mgb-2">exemple => display : block;</p>
		</div>

		<div class="exemple">

			<p class="green-900 mgb-4">we use span because it's an inline element</p>
			<!-- start exemple -->
			<div>
				<p class="mgb-4 mgt-4">before display block :</p>
				<span class="pd-2 bg-yellow-500">span</span>
				<span class="pd-2 bg-yellow-500">span</span>
				<span class="pd-2 bg-yellow-500">span</span>
				<p class="mgb-4 mgt-4">after display block :</p>
				<span class="pd-2 bg-yellow-500 block mgt-1">span</span>
				<span class="pd-2 bg-yellow-500 block mgt-1">span</span>
				<span class="pd-2 bg-yellow-500 block mgt-1">span</span>
			</div>
		</div>
		<!-- exemple -->
		<div>
			<p class="font-3x mgt-2 mgb-2">exemple => display : flex;</p>
		</div>

		<div class="exemple">
		
			<p class="green-900 mgb-4">we use p because it's an block element</p>
			<!-- start exemple -->
			<div>
				<p class="mgb-4 mgt-4">before display flex :</p>
				<p class="pd-2 bg-yellow-500 mgt-1">p tag</p>
				<p class="pd-2 bg-yellow-500 mgt-1">p tag</p>
				<p class="pd-2 bg-yellow-500 mgt-1">p tag</p>
				<p class="mgb-4 mgt-4">after display flex :</p>
				<div class="flex">
					<p class="pd-2 bg-yellow-500 mgr-1">p tag</p>
					<p class="pd-2 bg-yellow-500 mgr-1">p tag</p>
					<p class="pd-2 bg-yellow-500 mgr-1">p tag</p>
				</div>
			</div>
		</div>
		<!-- exemple -->
		<div>
			<p class="font-3x mgt-2 mgb-2">exemple => display : none;</p>
		</div>

		<div class="exemple">
		
			<!-- start exemple -->
			<div>
				<p class="mgb-4 mgt-4">before display none :</p>
				<span class="pd-2 bg-yellow-500">span 1</span>
				<span class="pd-2 bg-yellow-500">span 2</span>
				<span class="pd-2 bg-yellow-500">span 3</span>
				<p class="mgb-4 mgt-4">after display none : we hide the first and the last element</p>
                
				<span class="pd-2 bg-yellow-500 none mgt-1">span 1</span>
				<span class="pd-2 bg-yellow-500 block mgt-1">span 2</span>
				<span class="pd-2 bg-yellow-500 none mgt-1">span 3</span>
			</div>
		</div>
	</div>
</div>

<style>
</style>
