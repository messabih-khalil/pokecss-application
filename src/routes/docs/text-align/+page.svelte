<script>
    import Code from '../../../components/Code.svelte'
</script>

<div>
    <div class="head">
		<p class="font-4x font-500  mgb-4">Text Alignment and Text Direction</p>
	</div>
    <div class="text-align">
        <p class="mgt-1">
            The <span class="yellow-400"> text-align </span> property is used to set the horizontal alignment
            of a text.
        </p>
        <p class="mgt-1">A text can be left or right aligned, centered.</p>
    
        <!-- classes -->
    
        <ul>
            <li>
                <p class="pd-2">
                    Center text : <span class="font-500 blue-400">text-center</span>
                </p>
                <Code
                    code='
    <p class="text-center">
        text center
    <p>
    
                    '
                />
            </li>
            <li>
                <p class="pd-2">
                    Left align : <span class="font-500 blue-400">text-left</span>
                </p>
                <Code
                    code='
    <p class="text-left">
        text center
    <p>
    
                    '
                />
            </li>
            <li>
                <p class="pd-2">
                    Right align : <span class="font-500 blue-400">text-right</span>
                </p>
                <Code
                    code='
    <p class="text-right">
        text center
    <p>
    
                    '
                />
            </li>
        </ul>
    
        <!-- text decoration -->
    </div>
    
</div>

<style>

</style>