<script>
    // import file from '../assets/pokecss.zip'
</script>

<!-- download button -->
<!--  -->
<a
	
	class="bg-yellow-400 download-button font-600 pdl-10 pdr-10 pdt-2 pdb-2 flex align-center br-2x-solid-black black"
	href={file}
    download="pokecss.zip"
>
	<i class="ri-download-2-line mgr-1" />
	<span> Download </span>
</a>


<style>
	.download-button {
			font-size: 1.2rem;
		}
	@media only screen and (max-width: 720px) {
		.download-button {
			display: none;
		}
	}
</style>
