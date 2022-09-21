<script>
	import Code from '../../../components/Code.svelte';
</script>

<div>
	<div class="head">
		<p class="font-4x font-500  mgb-4">Margins</p>
	</div>
	<div class="text-align">
		<p class="mgt-1">
			the shorthand property of margin : <span class="blue-400 font-500">mg"the side"-"size"</span>
		</p>

		<div class="types">
			<p class="font-3x mgt-2 font-400">Margins names :</p>
			<ul class="pdl-2">
				<li class="mgt-1">> mg : global margin</li>
				<li class="mgt-1">> mgt : margin-top</li>
				<li class="mgt-1">> mgb : margin-bottom</li>
				<li class="mgt-1">> mgl : margin-left</li>
				<li class="mgt-1">> mgr : margin-right</li>
			</ul>
		</div>

		<div class="types">
			<p class="font-3x mgt-2 font-400">Margin size :</p>
			<ul class="pdl-2">
				<li class="mgt-1">> From 1 to 10</li>
			</ul>
		</div>

		<!-- exemples -->

		<div class="exemples">
			<p class="font-3x mgt-2">
				Exemples : <span class="blue-400">mg-10</span>
			</p>
			<!-- code -->
			<Code
				code='
<div>
    <p class="bg-purple-400">
        Lorem
    </p>
    <p class="mg-10 bg-red-400">
        Margin box
    </p>
    <p class="bg-green-400">
        Lorem
    </p>
</div>
            '
			/>

			<p class="font-3x mgt-2">Result :</p>

			<div class="pdt-2 pdb-2">
                <p class="bg-purple-400">
                    Lorem
                </p>
                <p class="mg-10 bg-red-400">
                    Margin box
                </p>
                <p class="bg-green-400">
                    Lorem
                </p>
            </div>
	
			
		</div>

		<!-- exemples -->

		<div class="exemples">
			<p class="font-3x mgt-2">
				Exemples : <span class="blue-400">mgt-10</span>
			</p>
			<!-- code -->
			<Code
				code='
<div>
    <p class="bg-purple-400">
        Lorem
    </p>
    <p class="mgt-10 bg-red-400">
        Margin box
    </p>
    <p class="bg-green-400">
        Lorem
    </p>
</div>
            '
			/>

			<p class="font-3x mgt-2">Result :</p>

			<div class="pdt-2 pdb-2">
                <p class="bg-purple-400">
                    Lorem
                </p>
                <p class="mgt-10 bg-red-400">
                    Margin box
                </p>
                <p class="bg-green-400">
                    Lorem
                </p>
            </div>
	
			
		</div>

		<!-- exemples -->

		<div class="exemples">
			<p class="font-3x mgt-2">
				Exemples : <span class="blue-400">mgb-10</span>
			</p>
			<!-- code -->
			<Code
				code='
<div>
    <p class="bg-purple-400">
        Lorem
    </p>
    <p class="mgb-10 bg-red-400">
        Margin box
    </p>
    <p class="bg-green-400">
        Lorem
    </p>
</div>
            '
			/>

			<p class="font-3x mgt-2">Result :</p>

			<div class="pdt-2 pdb-2">
                <p class="bg-purple-400">
                    Lorem
                </p>
                <p class="mgb-10 bg-red-400">
                    Margin box
                </p>
                <p class="bg-green-400">
                    Lorem
                </p>
            </div>
	
			
		</div>

		<!-- exemples -->

		<div class="exemples">
			<p class="font-3x mgt-2">
				Exemples : <span class="blue-400">mgl-10</span>
			</p>
			<!-- code -->
			<Code
				code='
<div>
    <p class="bg-purple-400">
        Lorem
    </p>
    <p class="mgl-10 bg-red-400">
        Margin box
    </p>
    <p class="bg-green-400">
        Lorem
    </p>
</div>
            '
			/>

			<p class="font-3x mgt-2">Result :</p>

			<div class="pdt-2 pdb-2">
                <p class="bg-purple-400">
                    Lorem
                </p>
                <p class="mgl-10 bg-red-400">
                    Margin box
                </p>
                <p class="bg-green-400">
                    Lorem
                </p>
            </div>
	
			
		</div>

		<!-- exemples -->

		<div class="exemples">
			<p class="font-3x mgt-2">
				Exemples : <span class="blue-400">mgr-10</span>
			</p>
			<!-- code -->
			<Code
				code='
<div>
    <p class="bg-purple-400">
        Lorem
    </p>
    <p class="mgr-10 bg-red-400">
        Margin box
    </p>
    <p class="bg-green-400">
        Lorem
    </p>
</div>
            '
			/>

			<p class="font-3x mgt-2">Result :</p>

			<div class="pdt-2 pdb-2">
                <p class="bg-purple-400">
                    Lorem
                </p>
                <p class="mgr-10 bg-red-400">
                    Margin box
                </p>
                <p class="bg-green-400">
                    Lorem
                </p>
            </div>
	
			
		</div>
	</div>
</div>

<style>
	
</style>
