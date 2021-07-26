<script context="module">
	import Header from '$lib/header/Header.svelte';

	import { browser, dev } from '$app/env';

	// we don't need any JS on this page, though we'll load
	// it in dev so that we get hot module replacement...
	export const hydrate = dev;

	// ...but if the client-side router is already loaded
	// (i.e. we came here from elsewhere in the app), use it
	export const router = browser;

	// since there's no dynamic data here, we can prerender
	// it so that it gets served as a static asset in prod
	export const prerender = true;
</script>

<Header />

<div class="jumbotron jumbotron-fluid">
	<div class="container">
		<div class="card">
			<div class="card-header">
				<h1 class="display-5">About Me, personally 😎</h1>
			</div>
			<div class="card-body">
				<div class="lead">
					<p>
						Hi there, I'm Justin a 2nd year student at Swinburne University doing Bachelor of Computer Science 
						majoring in Software & Game Development. Currently learning svelte, Node.js and Express.js. Pasionate 
						about automating stuff whether if it's neccessary or not 🤪, and creating new projects ever-so-often even 
						though I lost intrest way to quickly. My hobbies include playing video games 😎 <em>&lpar;mostly the 
						simulators kind&rpar;</em>, listening to music <em>&lpar;enjoyed any kind of genre, but mostly listening 
						to EDM, POP, K-POP & J-POP&rpar;</em>, and binge watching TV shows <em>&lpar; mainly the triller and crime 
						ones. Oh so good&rpar;</em>.
					</p>
				</div>
			</div>
		</div>
		<br>
		<div class="card">
			<div class="card-header">
				<h1 class="display-5">About this site</h1>
			</div>
			<div class="card-body">
				<div class="lead">
					<p>
						This website is built using Svelte & Bootstrap 5.0 for the frontend and using node.js & express.js for the backend.
						Website repo can be found <a href="https://github.com/SanJeosutin/sanjustin.xyz" target="_blank">on My Github</a>.
						Current hour&lpar;s&rpar; <del>wasted</del> spent: <strong>~4</strong>
					</p>
				</div>
			</div>
		</div>
	</div>
</div>