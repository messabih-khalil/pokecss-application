<script>
	// import css
	import '../../assets/main.css';

	import Navbar from '../../components/Navbar.svelte';
	import Menu from '../../components/Menu.svelte';
</script>

<Navbar />
<body class="bg-grey-100">
	<div class="layout">
		<div class="menu">
			<Menu />
		</div>
		<main class="pdb-5 pdl-5 pdr-5">
			<slot />
		</main>
	</div>
</body>

<style>
	.layout {
		display: grid;
		grid-template-columns: 18% 82%;
	}
	main {
		padding-top: 8rem;
	}
	@media only screen and (min-width: 980px) and (max-width: 1200px) {
		.layout {
			grid-template-columns: 20% 80%;
		}
	}

	@media only screen and (min-width: 721px) and (max-width: 979px) {
		.layout {
			grid-template-columns: 25% 75%;
		}
	}

	@media only screen and (max-width: 720px) {
		.layout {
			display: block;
		}

		.layout .menu {
			width: 600px;
		}
	}
</style>
