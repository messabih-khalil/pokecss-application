<script>
	import Code from '../../../components/Code.svelte';
</script>

<div>
	<div class="head">
		<p class="font-4x font-500  mgb-4">Columns</p>
	</div>
	<div class="text-align">
		<p class="mgt-1">
			Columns help you to make web designe responsive and work as well in many devices like : <span
				class="font-500">Smart phones - Tablet - Laptop - Destop computer ...</span
			>
		</p>

		<!-- text decoration -->
		<div class="types">
			<p class="font-3x mgt-2 font-400">How To write Columns :</p>
			<p>- First of all we need to create div with class "row"</p>
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
<div class="row gap-1">
    <div class="xl-2 lg-3 md-4 sm-5 xs-6">
        <p>
            Div 1
        </p>
    </div>
    <div class="xl-2 lg-3 md-4 sm-5 xs-6">
        <p>
            Div 2
        </p>
    </div>
    <div class="xl-2 lg-3 md-4 sm-5 xs-6">
        <p>
            Div 3
        </p>
    </div>
    <div class="xl-2 lg-3 md-4 sm-5 xs-6">
        <p>
            Div 4
        </p>
    </div>
    <div class="xl-2 lg-3 md-4 sm-5 xs-6">
        <p>
            Div 5
        </p>
    </div>
    <div class="xl-2 lg-3 md-4 sm-5 xs-6">
        <p>
            Div 6
        </p>
    </div>
</div>

                    '
			/>
            <p class="font-3x mgb-2">Result : </p>
            <div class="row gap-1">
                <div class="xl-2 lg-3 md-4 sm-5 xs-6 bg-green-500 pd-2">
                    <p>
                        Div 1
                    </p>
                </div>
                <div class="xl-2 lg-3 md-4 sm-5 xs-6 bg-green-500 pd-2">
                    <p>
                        Div 2
                    </p>
                </div>
                <div class="xl-2 lg-3 md-4 sm-5 xs-6 bg-green-500 pd-2">
                    <p>
                        Div 3
                    </p>
                </div>
                <div class="xl-2 lg-3 md-4 sm-5 xs-6 bg-green-500 pd-2">
                    <p>
                        Div 4
                    </p>
                </div>
                <div class="xl-2 lg-3 md-4 sm-5 xs-6 bg-green-500 pd-2">
                    <p>
                        Div 5
                    </p>
                </div>
                <div class="xl-2 lg-3 md-4 sm-5 xs-6 bg-green-500 pd-2">
                    <p>
                        Div 6
                    </p>
                </div>
            </div>
            
		</div>
		<!-- exemples -->
		<div>
			<p class="font-3x mgt-2 mgb-1">Exemples :</p>
			<Code
				code='
<div class="row gap-3">
    <div class="xl-6 lg-7 md-12 sm-4 xs-12 bg-green-500 pd-2">
        <p>
            Div 1
        </p>
    </div>
    <div class="xl-5 lg-4 md-5 sm-7 xs-4 bg-green-500 pd-2">
        <p>
            Div 2
        </p>
    </div>
    <div class="xl-12 lg-8 md-6 sm-12 xs-7 bg-green-500 pd-2">
        <p>
            Div 3
        </p>
    </div>
    
</div>

                    '
			/>
            <p class="font-3x mgb-2">Result : </p>
            <div class="row gap-3">
                <div class="xl-6 lg-7 md-12 sm-4 xs-12 bg-green-500 pd-2">
                    <p>
                        Div 1
                    </p>
                </div>
                <div class="xl-5 lg-4 md-5 sm-7 xs-4 bg-green-500 pd-2">
                    <p>
                        Div 2
                    </p>
                </div>
                <div class="xl-12 lg-8 md-6 sm-12 xs-7 bg-green-500 pd-2">
                    <p>
                        Div 3
                    </p>
                </div>
               
            </div>
            
		</div>
	</div>
</div>

<style>
</style>
