<script>
	import { page } from "$app/stores";
	import logo from "./svelte-logo.svg";
</script>

<svelte:head>
	<title>San Justin</title>
</svelte:head>

<nav class="navbar navbar-expand-md navbar-light">
	<div class="background"></div>
	<div class="container d-flex justify-content-center bg-text">
		<div class="row">
			<div class="col" id="navBarAlt">
				<ul class="navbar-nav mr-auto" class:active={$page.path === '/projects'}>
					<li class="nav-item">
						<div class="text-font"> <a class="nav-item nav-link" sveltekit:prefetch href="/projects">Projects</a></div>
					</li>
					
					<li class="nav-item" class:active={$page.path === '/design'}>
						<div class="text-font"> <a class="nav-item nav-link" sveltekit:prefetch href="/designs">Designs</a></div>
					</li>
				</ul>
			</div>
			<div class="col" class:active={$page.path === '/'}>
				<a class="navbar-brand font-weight-bold logo-font" sveltekit:prefetch href="/">San Justin</a>
			</div>
			
			<div class="col" id="navBarAlt">
				<ul class="navbar-nav ml-auto">
					<li class="nav-item" class:active={$page.path === '/about'}>
						<div class="text-font"> <a class="nav-item nav-link" sveltekit:prefetch href="/about">About</a></div>
					</li>
					<li class="nav-item" class:active={$page.path === '/contact'}>
						<div class="text-font"> <a class="nav-item nav-link" sveltekit:prefetch href="/contact">Contact</a></div>
					</li>
				</ul>
			</div>
		</div>
	</div>
</nav>
