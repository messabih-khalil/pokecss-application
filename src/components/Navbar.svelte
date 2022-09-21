<script>
	import pokeLogo from '../assets/logo.png';
	import DownloadButton from './DownloadButton.svelte';
</script>

<!-- navbar -->
<nav>
	<div class="navbar fixed z-10 flex align-center justify-space-between">
		<div class="pdl-4 pdr-4 flex align-center justify-space-between pdt-1 pdb-1 navbar-items">
			<!-- logo -->
			<a class="logo flex align-center" href="/">
				<!-- logo image -->
				<img src={pokeLogo} alt="" />
			</a>
			<!-- button section -->
			<div class="flex align-center">
				<!-- github icon -->
				<a
					class="bg-yellow-400 github-source font-2x font-600 pdl-3 pdr-3 pd-1 pdb-1 flex align-center mgr-2 br-2x-solid-black black"
					href="https://github.com/messabih-khalil/pokecss-application"
				>
					<i class="ri-github-fill mgr-1 font-3x" />
					<span> Source </span>
				</a>

				<DownloadButton />
			</div>
		</div>
	</div>
</nav>

<style>
	nav {
		height: 10vh;
	}
	.navbar {
		width: 100%;
		height: 10vh;
		background-color: rgb(255, 255, 255);
		border-bottom: 1px solid rgb(200, 200, 200);
	}
	.navbar-items {
		width: 100%;
	}
	.logo {
		width: 120px;
	}

	@media only screen and (max-width: 720px) {
		.github-source{
			padding: 0;
			margin: 0;
			background-color: transparent;
			border: none;
			
		}
		.github-source i{
			color: #2770e6;
			font-size: 32px;
			margin: 0;
		}
		.github-source span{
			display: none;
		}
	}
</style>
