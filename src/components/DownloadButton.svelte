<script>
    import file from '../assets/pokecss.zip'
</script>

<!-- download button -->
<a
	class="bg-yellow-400 download-button font-2x font-600 pdl-3 pdr-3 pd-1 pdb-1 flex align-center br-2x-solid-black black"
	href={file}
    download="pokecss.zip"
>
	<i class="ri-download-2-line mgr-1" />
	<span> Download </span>
</a>


<style>
	@media only screen and (max-width: 720px) {
		.download-button {
			display: none;
		}
	}
</style>
