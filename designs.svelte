<script context="module">
	import Header from '$lib/header/Header.svelte';
	import { browser, dev } from '$app/env';

	export const hydrate = dev;
	export const router = browser;
	export const prerender = true;
</script>

<Header />

<div class="jumbotron jumbotron-fluid">
	<div class="container">
		<div class="card">
			<div class="card-header">
				<h1 class="display-5">Design Portfolio</h1>
			</div>
			<div class="card-body">
				<div class="lead">
					<p>
						Some stuff that I've worked on for the past few years or so. Or during my Uni year :D
					</p>
					<!--REAL CONTENT-->
					<div class="card-deck">

						<div class="row">
							<div class="col">
								<div class="card card-content">
									<img class="card-img-top" src="_temp-image-card-placeholder.svg" alt="Card image cap">
									<div class="card-body">
										<h5 class="card-title">Card title</h5>
										<p class="card-text">This is a wider card with supporting text below as a natural lead-in to additional content. This content is a little bit longer.</p>
									</div>
									<div class="card-footer">
										<a href="" class="btn btn-primary">Live Demo</a>
                                		<a href="" class="btn btn-secondary">Source Code</a>
									</div>
								  </div>
							</div>

							<div class="col">
								<div class="card card-content">
									<img class="card-img-top" src="_temp-image-card-placeholder.svg" alt="Card image cap">
									<div class="card-body">
										<h5 class="card-title">Card title</h5>
										<p class="card-text">This is a wider card with supporting text below as a natural lead-in to additional content. This content is a little bit longer.</p>
									</div>
									<div class="card-footer">
										<a href="" class="btn btn-primary">Live Demo</a>
                                		<a href="" class="btn btn-secondary">Source Code</a>
									</div>
								  </div>
							</div>

						</div>
						
						<br>

						<div class="row">
							<div class="col">
								<div class="card card-content">
									<img class="card-img-top" src="_temp-image-card-placeholder.svg" alt="Card image cap">
									<div class="card-body">
										<h5 class="card-title">Card title</h5>
										<p class="card-text">This is a wider card with supporting text below as a natural lead-in to additional content. This content is a little bit longer.</p>
									</div>
									<div class="card-footer">
										<a href="" class="btn btn-primary">Live Demo</a>
                                		<a href="" class="btn btn-secondary">Source Code</a>
									</div>
								  </div>
							</div>

							<div class="col">
								<div class="card card-content">
									<img class="card-img-top" src="_temp-image-card-placeholder.svg" alt="Card image cap">
									<div class="card-body">
										<h5 class="card-title">Card title</h5>
										<p class="card-text">This is a wider card with supporting text below as a natural lead-in to additional content. This content is a little bit longer.</p>
									</div>
									<div class="card-footer">
										<a href="" class="btn btn-primary">Live Demo</a>
                                		<a href="" class="btn btn-secondary">Source Code</a>
									</div>
								  </div>
							</div>

						</div>

					</div>
					<!--REAL CONTENT-->
				</div>
			</div>
		</div>
	</div>
</div>
<br>
<br>
<br>

<style>
	.card-content{
		width: 20rem;
	}

	.card-deck{
		margin: 0px 65px;
	}

	.card-footer{
		padding-left: 44px;
	}
</style>