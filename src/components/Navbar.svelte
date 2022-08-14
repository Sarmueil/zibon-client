<script lang="ts">
	let showSidebar = false;
</script>

<svelte:head>
	<link rel="stylesheet" href="https://unicons.iconscout.com/release/v4.0.0/css/line.css" />
</svelte:head>

<nav>
	<div class="container nav__container">
		<a href="/">
			<img src="/images/zibonLogo.png" alt="Header_logo" class="nav__logo" />
		</a>
		<ul class="nav__linkss">
			<li><a href="#about">About</a></li>
			<li><a href="#features">Featured</a></li>
			<li><a href="#download">Download</a></li>
			<li><a href="/#">Request Demo</a></li>
		</ul>

		{#if showSidebar}
			<ul class="nav__links" on:click={()=> showSidebar = !showSidebar}>
				<li><a href="#about">About</a></li>
				<li><a href="#features">Featured</a></li>
				<li><a href="#download">Download</a></li>
				<li><a href="/#">Request Demo</a></li>
			</ul>
		{/if}

		<ul class="nav__socials">
			<li><a href="/"><i class="uil uil-instagram-alt" /></a></li>
			<li><a href="/"><i class="uil uil-twitter" /></a></li>
			<li><a href="/"><i class="uil uil-instagram-alt" /></a></li>
		</ul>

		<button class="nav__toggle-btn" on:click={()=> showSidebar = !showSidebar}><i class="uil uil-bars" /></button>
		<!-- {#if !showSidebar}
			<button class="nav__toggle-btn" id="nav__toggle-close"><i class="uil uil-multiply" /></button>
		{/if} --> 
	</div>
</nav>

<style>
	nav {
		height: calc(16px * 5);
		width: 100vw;
		display: grid;
		place-items: center;
		position: fixed;
		top: 0;
		left: 0;
		z-index: 99;
		background: linear-gradient(to right, #141e30, #243b55);
		box-shadow: 0 0.1rem 0.1rem rgba(0, 0, 0, 0.4);
	}
	.nav__container {
		height: 100%;
		display: flex;
		justify-content: space-between;
		align-items: center;
	}
	.nav__toggle-btn {
		display: none;
	}
	.nav__logo {
		width: 7.5rem;
	}
	.nav__links {
		display: flex;
		gap: 4rem;
		font-weight: 300;
	}
	.nav__linkss {
		display: flex;
		gap: 4rem;
		font-weight: 300;
	}
	.nav__socials {
		display: flex;
		gap: 1rem;
	}
	.nav__socials a {
		width: 2rem;
		height: 2rem;
		display: grid;
		background-color: #eb9d2f;
		border-radius: 0.5rem;
		color: #243b55;
		place-items: center;
	}
	.nav__socials a:hover {
		box-shadow: 0 1rem 1rem rgba(0, 0, 0, 0.4);
	}

	@media screen and (max-width: 1024px) {
		.nav__socials {
			display: none;
		}
		.nav__links {
			position: absolute;
			top: 100%;
			right: 0;
			flex-direction: column;
			gap: 0;
			/* display: none; */
			/* background: #eb9d2f; */
		}
		.nav__linkss {
			display: none;
		}
		.nav__links li {
			height: 5rem;
			box-shadow: -3rem 3rem 3rem rgba(0, 0, 0, 0.7);
			animation: navAnimation 600ms ease forwards;
			transform: rotateX(90deg);
			opacity: 0;
			transform-origin: top;
		}
		.nav__links li:nth-child(2) {
           animation-delay: 200ms;
		}
		.nav__links li:nth-child(3) {
           animation-delay: 400ms;
		}
		.nav__links li:nth-child(4) {
           animation-delay: 600ms;
		}

		@keyframes navAnimation {
			to {
				transform: rotateX(0);
				opacity: 1;
			}
		}
		.nav__links li a {
			background: #141e30;
			height: 100%;
			width: 100%;
			display: flex;
			align-items: center;
			padding: 1rem 5rem 1rem 3rem;
			border-top: 1px solid #243b55;
			transition: all 400ms ease;
		}
		.nav__toggle-btn {
			display: inline-block;
			font-size: 2rem;
			background: transparent;
			cursor: pointer;
			color: white;
		}
		/* #nav__toggle-close {
			display: none;
		} */
	}
</style>
