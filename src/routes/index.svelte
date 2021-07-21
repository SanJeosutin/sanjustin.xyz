<script context="module">
	import { page } from '$app/stores';
	export const prerender = true;
</script>

<section>
	<div id="topLayer">
		<!--MAIN CONTENT-->
		<div class="row h-100">
			<div class="col-sm-12 my-auto">
				<div class="card-body text-font">
					<h1 class="card-title title text-center">San Justin</h1>
					<ul class="nav nav-tabs card-header-tabs justify-content-center">
						<li class="nav-item" class:active={$page.path === '/projects'}>
							<a class="nav-link" sveltekit:prefetch href="/projects">Projects</a>
						</li>
						<li class="nav-item" class:active={$page.path === '/about'}>
							<a class="nav-link" sveltekit:prefetch href="/about">About</a>
						</li>
						<li class="nav-item" class:active={$page.path === '/designs'}>
							<a class="nav-link" sveltekit:prefetch href="/designs">Designs</a>
						</li>
					</ul>
				</div>
			</div>
		</div>
	</div>
</section>

<style>
	.title{
		opacity: 90%;
		text-shadow: 7px 7px 16px #0F0000;
		font: 8vw 'Sriracha', cursive;
    	user-select: none;
	}

	.text-font{
    	font: 1.75em 'Sriracha', cursive;
	}

	:global(.text-font a){
		color: #6c757d;
		display: inline-block;
  		vertical-align: middle;
  		-webkit-transform: perspective(1px) translateZ(0);
  		transform: perspective(1px) translateZ(0);
  		box-shadow: 0 0 1px rgba(0, 0, 0, 0);
  		-webkit-transition-duration: 0.3s;
  		transition-duration: 0.3s;
  		-webkit-transition-property: transform;
  		transition-property: transform;
	}

	:global(.text-font a:hover), :global(.text-font a:focus), :global(.text-font a:active) {
		border: none;
		text-decoration: none;
		-webkit-transform: scale(1.1);
  		transform: scale(1.1);
		color: #f0f8ff;
	}
</style>
