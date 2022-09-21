<script>
	import Code from '../../../components/Code.svelte';
</script>

<div>
	<div class="head">
		<p class="font-4x font-500  mgb-4">Positions</p>
	</div>
	<div class="text-align">
		<p class="mgt-1">
			the shorthand property of margin : <span class="blue-400 font-500">"type of positions"</span>
		</p>

		<div class="types">
			<p class="font-3x mgt-2 font-400">Position types :</p>
			<ul class="pdl-2">
				<li class="mgt-1">> fixed => position : fixed;</li>
				<li class="mgt-1">> relative => position : relative;</li>
				<li class="mgt-1">> absolute => position : absolute;</li>
				<li class="mgt-1">> static => position : static;</li>
				<li class="mgt-1">> sticky => position : sticky;</li>
			</ul>
		</div>

		<!-- exemples -->

		<p class="font-3x mgt-2">position: static; :</p>

		<p class="pdl-2 mgt-1">
			HTML elements are positioned static by default. Static positioned elements are not affected by
			the top, bottom, left, and right properties.
		</p>
		<!-- exemples -->

		<p class="font-3x mgt-2">position: relative; :</p>

		<p class="pdl-2 mgt-1">
			An element with <span class="blue-500">"relative"</span> class name is positioned relative to its
			normal position. Setting the top, right, bottom, and left properties of a relatively-positioned
			element will cause it to be adjusted away from its normal position. Other content will not be adjusted
			to fit into any gap left by the element.
		</p>
		<!-- exemples -->

		<p class="font-3x mgt-2">position: fixed; :</p>

		<p class="pdl-2 mgt-1">
			An element with <span class="blue-500">"fixed"</span> class name is positioned relative to the
			viewport, which means it always stays in the same place even if the page is scrolled. The top,
			right, bottom, and left properties are used to position the element. A fixed element does not leave
			a gap in the page where it would normally have been located.
		</p>
		<!-- exemples -->

		<p class="font-3x mgt-2">position: absolute; :</p>

		<p class="pdl-2 mgt-1">
			An element with <span class="blue-500">"absolute"</span> class name is positioned relative to the
			nearest positioned ancestor (instead of positioned relative to the viewport, like fixed). However;
			if an absolute positioned element has no positioned ancestors, it uses the document body, and moves
			along with page scrolling.
		</p>
		<!-- exemples -->

		<p class="font-3x mgt-2">position: sticky; :</p>

		<p class="pdl-2 mgt-1">
			An element with <span class="blue-500">"sticky"</span> class name is positioned based on the user's
			scroll position. A sticky element toggles between relative and fixed, depending on the scroll position.
			It is positioned relative until a given offset position is met in the viewport - then it "sticks"
			in place (like position:fixed).
		</p>
	</div>
</div>

<style>
</style>
