<script>
	import '../app.css';
</script>

<main>
	<slot />
</main>

<div class="background fixed-bottom"></div>
<footer class="fixed-bottom" align="center">
		<p>
			<strong>&blacktriangleleft;</strong>
			<a class="fab fa-github" href="https://github.com/SanJeosutin?tab=repositories">{@html '&ThickSpace;'}<i> Github </i></a>  |
			<a class="fab fa-linkedin-in" href="https://www.linkedin.com/in/justin-santoso-8467b0200/">{@html '&ThickSpace;'}<i> LinkedIn </i></a>  |
			<a class="fas fa-envelope" href="mailto:contact.sanjustin@gmail.com">{@html '&ThickSpace;'}<i style="font-weight: normal;"> Contact Me </i></a>
			<strong>&blacktriangleright;</strong>
		</p>
</footer>

<style>
	main {
		flex: 1;
		display: flex;
		flex-direction: column;
		padding: 1rem;
		width: 100%;
		max-width: 1024px;
		margin: 0 auto;
		box-sizing: border-box;
	}

	footer i{
		font-family: 'Open Sans', sans-serif;
	}

	footer a{
		color: #2e2e2e;
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

	footer a:hover, footer a:focus, footer a:active {
		border: none;
		text-decoration: none;
		-webkit-transform: scale(1.1);
  		transform: scale(1.1);
		color: #0088ff;
	}


	@media (min-width: 480px) {
		footer {
			padding: 40px 0;
		}
	}
</style>
