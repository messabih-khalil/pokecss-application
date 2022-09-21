<script>
	import Code from '../../../components/Code.svelte';
</script>

<div>
	<div class="head">
		<p class="font-4x font-500  mgb-4">Grid system</p>
	</div>
	<div class="text-align">
		<p class="mgt-1">
			Grid system Also help you to make designe responsive but the main diffrence between <span class="font-700">"Columns"</span>  and  <span class="font-700">"Grid-system"</span>: <span
				class="font-500">write the number of columns in diffrent devices and the children share the columns equally </span
			>
		</p>

		
		<div class="types">
			<p class="font-3x mgt-2 font-400">How To write Grid system :</p>
			<p>- Add this pattern in parrent div who hold the children : <span class="font-600">grid-"device"-"number of columns"</span></p>
			<p>- Secend add number of column in every specefic device size :</p>
			<ul class="pdl-2">
				<li>- xs : extra small devices</li>
				<li>- sm : small devices</li>
				<li>- md : medium devices</li>
				<li>- lg : large devices</li>
				<li>- xl : extra large devices</li>
			</ul>
			<p>- Third adding gap between columns:</p>
			<ul class="pdl-2">
				<li>- gap-1</li>
				<li>- gap-2</li>
				<li>- gap-3</li>
				<li>- gap-4</li>
			</ul>
		</div>
		<!-- exemples -->
		<div>
			<p class="font-3x mgt-2 mgb-1">Exemples :</p>
			<Code
				code='
<div class="grid-xl-8 grid-lg-6 grid-md-5 grid-sm-3 grid-xs-1 gap-1">
    <div>
        <p>
            Div 1
        </p>
    </div>
 
    <div>
        <p>
            Div 2
        </p>
    </div>
 
    <div>
        <p>
            Div 3
        </p>
    </div>
 
    <div>
        <p>
            Div 4
        </p>
    </div>
 
    <div>
        <p>
            Div 5
        </p>
    </div>
 
    <div>
        <p>
            Div 6
        </p>
    </div>
 
    <div>
        <p>
            Div 7
        </p>
    </div>
 
    <div>
        <p>
            Div 8
        </p>
    </div>
 
</div>

                    '
			/>
            <p class="font-3x mgb-2">Result : </p>
            <div class="grid-xl-8 grid-lg-6 grid-md-5 grid-sm-3 grid-xs-1 gap-1">
                <div class="pd-2 bg-yellow-500">
                    <p>
                        Div 1
                    </p>
                </div>
             
                <div class="pd-2 bg-yellow-500">
                    <p>
                        Div 2
                    </p>
                </div>
             
                <div class="pd-2 bg-yellow-500">
                    <p>
                        Div 3
                    </p>
                </div>
             
                <div class="pd-2 bg-yellow-500">
                    <p>
                        Div 4
                    </p>
                </div>
             
                <div class="pd-2 bg-yellow-500">
                    <p>
                        Div 5
                    </p>
                </div>
             
                <div class="pd-2 bg-yellow-500">
                    <p>
                        Div 6
                    </p>
                </div>
             
                <div class="pd-2 bg-yellow-500">
                    <p>
                        Div 7
                    </p>
                </div>
             
                <div class="pd-2 bg-yellow-500">
                    <p>
                        Div 8
                    </p>
                </div>
             
            </div>
            
		</div>
	
		
	</div>
</div>

<style>
</style>
