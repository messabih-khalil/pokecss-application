<script>
	import Code from '../../../components/Code.svelte';
</script>

<div>
	<div class="head">
		<p class="font-4x font-500  mgb-4">Border</p>
	</div>
	<div class="text-align">
		<p class="mgt-1">
			the shorthand property class to add border is look like: <span class="blue-400 font-500"
				>br"border side"-"border thickness"-"border type"-"border color"</span
			>
		</p>

		<!--  decoration -->
		<div class="types">
			<p class="font-3x mgt-2 font-400">Borders type :</p>
			<ul class="pdl-2">
				<li class="mgt-1">> dotted - Defines a dotted border</li>
				<li class="mgt-1">> dashed - Defines a dashed border</li>
				<li class="mgt-1">> solid - Defines a solid border</li>
				<li class="mgt-1">> double - Defines a double border</li>
				<li class="mgt-1">> groove - Defines a 3D grooved border. The effect depends on the border-color value</li>
				<li class="mgt-1">> ridge - Defines a 3D ridged border. The effect depends on the border-color value</li>
				<li class="mgt-1">> inset - Defines a 3D inset border. The effect depends on the border-color value</li>
				<li class="mgt-1">> outset - Defines a 3D outset border. The effect depends on the border-color value</li>
				<li class="mgt-1">> none - Defines no border</li>
				<li class="mgt-1">> hidden - Defines a hidden border</li>
			</ul>

			
		</div>
        <!--  thickness -->
        <div class="types">
			<p class="font-3x mgt-2 font-400">Border side:</p>
			<ul class="pdl-2">
				<li class="mgt-1">> Top : t</li>
				<li class="mgt-1">> Bottom : b</li>
				<li class="mgt-1">> Left : l</li>
				<li class="mgt-1">> right : r</li>
				
			</ul>

			<p class="mgt-2">the first part of the shorthand property is the side of the border , <span class="font-500 green-900">Notice : if you want to put global border dont specify the border side </span> </p>
			<p class="mgt-1">
				exemple : <span class="blue-400 font-500"
					>br-2x-dotted-"border color"
				</span>
			</p>
		</div>
        
        <!-- color -->
        <div class="types">
			<p class="font-3x mgt-2 font-400">Border Color:</p>
			<ul class="pdl-2">
				<li class="mgt-1">> to add the color, only flow the pattern "color"-"brightness" exemple : <span class="red-500">red-500</span></li>
			</ul>

			<p class="mgt-2">add border color </p>
			<p class="mgt-1">
				exemple : <span class="blue-400 font-500"
					>br-2x-dotted-red-500
				</span>
			</p>
		</div>
        <!-- exemple -->
        <p class="font-3x mgt-2 mgb-2">
            Exemple :  <span class="grey-700">add border top with red color</span>
        </p>

        <Code code='
<div class="brt-5x-dotted-red-500">
    <p>
        Exemple
    </p>
</div>
        ' />

        <!-- exemple -->
        <p class="font-3x mgb-2">
            Result : 
        </p>
        <div class="brt-5x-dotted-red-500">
            <p class="font-3x">
                Exemple
            </p>
        </div>
        <!-- exemple -->
        <p class="font-3x mgt-2 mgb-2">
            Exemple :  <span class="grey-700">add border bottom with blue color</span>
        </p>

        <Code code='
<div class="brb-5x-solid-blue-500">
    <p>
        Exemple
    </p>
</div>
        ' />

        <!-- exemple -->
        <p class="font-3x mgb-2">
            Result : 
        </p>
        <div class="brb-5x-solid-blue-500">
            <p class="font-3x">
                Exemple
            </p>
        </div>
        <!-- exemple -->
        <p class="font-3x mgt-2 mgb-2">
            Exemple :  <span class="grey-700">add border left with green color</span>
        </p>

        <Code code='
<div class="brl-5x-dashed-green-500">
    <p>
        Exemple
    </p>
</div>
        ' />

        <!-- exemple -->
        <p class="font-3x mgb-2">
            Result : 
        </p>
        <div class="brl-5x-dashed-green-500 pdl-1">
            <p class="font-3x">
                Exemple
            </p>
        </div>
        <!-- exemple -->
        <p class="font-3x mgt-2 mgb-2">
            Exemple :  <span class="grey-700">add border right with purple color</span>
        </p>

        <Code code='
<div class="brr-5x-doubple-purple-500">
    <p>
        Exemple
    </p>
</div>
        ' />

        <!-- exemple -->
        <p class="font-3x mgb-2">
            Result : 
        </p>
        <div class="brr-5x-double-purple-500">
            <p class="font-3x">
                Exemple
            </p>
        </div>
        <!-- exemple -->
        <p class="font-3x mgt-2 mgb-2">
            Exemple :  <span class="grey-700">add global border with yellow color</span>
        </p>

        <Code code='
<div class="br-5x-solid-yellow-500">
    <p>
        Exemple
    </p>
</div>
        ' />

        <!-- exemple -->
        <p class="font-3x mgb-2">
            Result : 
        </p>
        <div class="br-5x-solid-yellow-500">
            <p class="font-3x pd-1">
                Exemple
            </p>
        </div>

	</div>
</div>

<style>
</style>
