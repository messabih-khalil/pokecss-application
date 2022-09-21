<script>
	// import css
	import '../assets/main.css';

	import pokeLogo from '../assets/logo.png';

	import 'remixicon/fonts/remixicon.css';

	import Navbar from '../components/Navbar.svelte';

	import DownloadButton from '../components/DownloadButton.svelte';

	import react from '../assets/tech-icons/react.png';
	import vue from '../assets/tech-icons/vue.png';
	import next from '../assets/tech-icons/next.png';
	import nuxt from '../assets/tech-icons/nuxt.png';
	import svelte from '../assets/tech-icons/svelte.png';
</script>

<div class="hidden body">
	<Navbar />
	<!-- hero main -->
	<div class="bg-yellow-400 hero">
		<div class="container hero-section flex align-center justify-center column">
			<div class="content text-center flex column justify-center align-center">
				<img src={pokeLogo} class="hero-image" alt="" />
				<span class="hero-text font-500">
					Free , open source library provides over then 390,000 css class
					<br />
					to customize and fast web interfaces design
				</span>
			</div>
			<!-- tech -->
			<div class="tech grid-xl-5 grid-lg-5 grid-md-5 grid-sm-5 grid-xs-5 gap-3 mgt-2 mgb-2">
				<div class="tech-image-box">
					<img src={react} alt="" />
				</div>
				<div class="tech-image-box">
					<img src={vue} alt="" />
				</div>
				<div class="tech-image-box">
					<img src={next} alt="" />
				</div>
				<div class="tech-image-box">
					<img src={nuxt} alt="" />
				</div>
				<div class="tech-image-box">
					<img src={svelte} alt="" />
				</div>
			</div>
			<!-- buttons -->

			<div class="buttons mgt-3 flex">
				<a
					class="download-button font-2x font-600 pdl-7 pdr-7 pd-1 pdb-1 flex align-center mgr-2 flex align-center white bg-black"
					href="/docs"
				>
					<i class="ri-git-repository-line mgr-1" />
					<span> Docs </span>
				</a>
				<DownloadButton />
			</div>
		</div>
	</div>
</div>

<style lang="scss">
	.body {
		height: 100vh;
	}
	.hero {
		height: 95vh;
	}

	.hero-section {
		height: 91vh;
	}

	.hero-text {
		font-size: 24px;
		margin: 1rem 0;
	}

	.hero-image {
		width: 400px;
	}

	.tech-image-box {
		height: 70px;
		width: 70px;
		display: flex;
		align-items: center;
		justify-content: center;
	}

	.tech-image-box img {
		width: 70px;
		height: 70px;
	}

	@media screen and (max-width: 420px) {
		.hero-image {
			width: 250px;
		}
		.tech {
			gap: 15px;
		}
		.tech-image-box {
			height: 50px;
			width: 50px;
		}

		.tech-image-box img {
			width: 50px;
			height: 50px;
		}
	}
	@media screen and (max-width: 320px) {
		.tech-image-box {
			height: 40px;
			width: 40px;
		}

		.tech-image-box img {
			width: 40px;
			height: 40px;
		}
	}
	@media screen and (max-width: 260px) {
		.hero-image {
			width: 200px;
		}
		.tech {
			display: none;
		}
	}
	@media (min-width: 421px) {
		.tech {
			gap: 15px;
		}
	}
</style>
