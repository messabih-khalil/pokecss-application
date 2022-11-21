<script>
	import { onMount } from 'svelte';

	import Navbar from '../components/Navbar.svelte';
	let menu = {
		Texts: ['text-align', 'text-decoration'],

		Fonts: ['font-size', 'font-weight', 'font-style'],
		'Color & Background': ['colors', 'backgrounds'],
		Spaces: ['paddings', 'margins'],
		'position & display': ['positions', 'display', 'overflow'],
		Responsive: ['columns', 'grid-system'],
		Border: ['borders' , 'radius']
	};
	let show = false;
	const showAndCloseMenu = (bool) => {
		show = bool;
		console.log(show);
	};
</script>

<div class="menu bg-yellow-400 z-5" class:show-menu={show}>
	<div class="menu-item pdt-5">
		{#each Object.entries(menu) as [key, value], index (key)}
			<li class="pdr-4 pdl-4 pdt-1 pdb-1">
				<span class="grey-500 font-2x font-600"> {key}</span>
				<ul>
					{#each value as v}
						<li class="pdl-1 mgt-1">
							<a href="/docs/{v}" class="black">
								{v}
							</a>
						</li>
					{/each}
				</ul>
			</li>
		{/each}
	</div>

	<!-- open -->

	<i
		class="ri-menu-unfold-line"
		on:click={() => showAndCloseMenu(true)}
		class:hide={show == true}
	/>
	<i
		class="ri-menu-fold-line"
		on:click={() => showAndCloseMenu(false)}
		class:hide={show == false}
	/>
</div>

<style>
	.menu {
		height: 90vh;
		position: fixed;
		width: 18%;
		transition: 0.5s;
		bottom: 0;
	}
	.menu-item {
		height: 90vh;
		overflow-y: scroll;
		position: relative;
	}

	.ri-menu-fold-line ,.ri-menu-unfold-line {
		background-color: #ffce58;
		width: fit-content;
		position: absolute;
		top: 50px;
		right: -30px;
		padding: 0.5rem;
		cursor: pointer;
		font-weight: 600;
		color: black;
		display: none;
	}
	.ri-menu-unfold-line.hide , .ri-menu-fold-line.hide {
		display: none;
	}
	@media only screen and (min-width: 980px) and (max-width: 1200px) {
		.menu {
			width: 20%;
		}
	}
	@media only screen and (min-width: 720px) and (max-width: 979px) {
		.menu {
			width: 25%;
		}
	}
	@media only screen and (max-width: 720px) {
		.menu {
			width: 200px;
			left: -200px;
		}
		.show-menu {
			left: 0px;
		}
		.ri-menu-fold-line ,.ri-menu-unfold-line {
			display: block;
		}
	}
</style>
