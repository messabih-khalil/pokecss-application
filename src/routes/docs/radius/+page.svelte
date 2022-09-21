<script>
	import Code from '../../../components/Code.svelte';
</script>

<div>
	<div class="head">
		<p class="font-4x font-500  mgb-4">Border</p>
	</div>
	<div class="text-align">
		<p class="mgt-1">
			the shorthand property class to add border radius is look like: <span class="blue-400 font-500"
				>radius-"radius size"</span
			>
		</p>

		<!--  decoration -->
		<div class="types">
			<p class="font-3x mgt-2 font-400">Radius size :</p>
			<ul class="pdl-2">
				<li class="mgt-1">> 1x</li>
				<li class="mgt-1">> 2x</li>
				<li class="mgt-1">> 3x</li>
				<li class="mgt-1">> until 10x</li>
				
			</ul>

			
		</div>
       



    
       
        <!-- exemple -->
        <p class="font-3x mgt-2 mgb-2">
            Exemple :  
        </p>

        <Code code='
<div class="brb-5x-solid-yellow-500 radius-2x">
    <p>
        Exemple
    </p>
</div>
<div class="brb-5x-solid-blue-500 radius-10x">
    <p>
        Exemple
    </p>
</div>
        ' />

     


    




        <!-- exemple -->
        <p class="font-3x mgb-2">
            Result : 
        </p>
        <div class="br-5x-solid-yellow-500 radius-2x">
            <p class="font-3x pd-1">
                Exemple
            </p>
        </div>
        <div class="br-5x-solid-blue-500 radius-10x mgt-4">
            <p class="font-3x pd-1">
                Exemple
            </p>
        </div>

	</div>
</div>

<style>
</style>
