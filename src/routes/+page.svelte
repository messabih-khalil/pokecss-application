<script>
	// import css
	import '../assets/main.css';

	import 'remixicon/fonts/remixicon.css';

	import Navbar from '../components/Navbar.svelte';

	import DownloadButton from '../components/DownloadButton.svelte';

</script>

<div class="hidden body">
	<Navbar />
	<!-- hero main -->
	<div class="hero">
		<div class="container hero-section flex align-center justify-center column">
			<div class="content text-center flex column justify-center align-center">
				<p class="header-hero">
					<span class="d-color">
						PokeCss </span> : make <span class="d-color">
							design
						</span> with simple <span class="d-color">
							css
						</span>Utility
					
				</p>
				<span class="hero-text font-500 grey-600">
					Free , open source library provides over then 390,000 css class
					<br />
					to customize and fast web interfaces design
				</span>
			</div>
			<!-- tech -->
			<div class="tech grid-xl-5 grid-lg-5 grid-md-5 grid-sm-5 grid-xs-5 gap-3 mgt-2 mgb-2">
				<div class="tech-image-box">
					<img src=https://github.com/get-icon/geticon/raw/master/icons/angular-icon.svg alt="" />
				</div>
				<div class="tech-image-box">
					<img src=https://github.com/get-icon/geticon/raw/master/icons/react.svg alt="" />
				</div>
				<div class="tech-image-box">
					<img src=https://github.com/get-icon/geticon/raw/master/icons/nextjs.svg alt="" />
				</div>
				<div class="tech-image-box">
					<img src=https://github.com/get-icon/geticon/raw/master/icons/vue.svg alt="" />
				</div>
				<div class="tech-image-box">
					<img src=https://github.com/get-icon/geticon/raw/master/icons/nuxt-icon.svg alt="" />
				</div>
			</div>
			<!-- buttons -->

			<div class="buttons mgt-3 flex">
				<a
					class="font-600 pdl-10 pdr-10 pdt-2 pdb-2 flex align-center mgr-2 flex align-center white bg-black"
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

	.header-hero{
		font-size: 4.5rem;
		font-weight: 700;
	}

	.d-color{
		background: linear-gradient(to right,#FFE031,#4dd0f8);
		background-size: 100%;
		background-clip: text;
		-webkit-background-clip: text;
		-moz-background-clip: text;
		-webkit-text-fill-color: transparent; 
		-moz-text-fill-color: transparent;
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

	.buttons a{
		font-size: 1.2rem;
	}

	@media screen and (max-width: 420px) {
		
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
