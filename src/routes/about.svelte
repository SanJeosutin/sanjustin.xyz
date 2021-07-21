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
		<h1 class="display-4">About</h1>
		<p class="lead">
			Hi there, I'm Justin the developer of this very website you've decided to visit. Yay! I've been working on web 
			development <em>(Back end ones)</em>for quite sometime now <em>(Around four years to be exact. Minus two years 
			focusing on<a href="https://www.vcaa.vic.edu.au/curriculum/vce/Pages/Index.aspx">VCE</a>. Yay Highschool...)</em>. 
			I'm now studying Computer Science at Swinburne, majoring in Software Design and Software Development. Now I'm on 
			my second year of Uni, I was hopping to refine my skills and knowlege during my time at Uni and meet like minded 
			people as well! I spend most of my time doing side projects, Uni assignments and working as kitchen hand casualy.
			I have listed all the units that I have done and some units that I will be taking for my current semester. 
		</p>
		<p class="lead">I've successfully completed the following units</p>
		<div class="container">
			<div class="row">
				<div class="col-sm-6">
					<div id="accordion1">
						<div class="card">
						  <div class="card-header " id="Semester1">
							<h5 class="mb-0">
							  <button class="btn btn-link collapsed" data-toggle="collapse" data-target="#collapseOne" aria-expanded="true" aria-controls="collapseOne">
								Semester 1
							  </button>
							</h5>
						  </div>
					  
						  <div id="collapseOne" class="collapse " aria-labelledby="Semester1" data-parent="#accordion1">
							<div class="card-body">
								<ul class=" list-group list-group-flush">
									<li class="list-group-item "><strong>-TNE10006</strong> Networks and Switching</li>
									<li class="list-group-item "><strong>-COS10003</strong> Computer & Logic Essentials</li>
									<li class="list-group-item "><strong>-COS10009</strong> Introduction to Programming</li>
									<li class="list-group-item "><strong>-COS10011</strong> Creating Web Applications</li>
								</ul>
							</div>
						  </div>
						</div>
					</div>
				</div>
				<br>
				<div class="col-sm-6">
					<div id="accordion2">
						<div class="card">
						  <div class="card-header " id="Semester2">
							<h5 class="mb-0">
							  <button class="btn btn-link collapsed" data-toggle="collapse" data-target="#collapseTwo" aria-expanded="false" aria-controls="collapseTwo">
								Semester 2
							  </button>
							</h5>
						  </div>
						  <div id="collapseTwo" class="collapse " aria-labelledby="Semester2" data-parent="#accordion2">
							<div class="card-body">
								<ul class=" list-group list-group-flush">
									<li class="list-group-item "><strong>-COS20001</strong> User-Centred Design</li>
									<li class="list-group-item "><strong>-COS20007</strong> Object Oriented Programming</li>
									<li class="list-group-item "><strong>-COS20015</strong> Fundamentals of Data Management</li>
									<li class="list-group-item "><strong>-COS30020</strong> Web Application Development</li>
								</ul>
							</div>
						  </div>
						</div>
					</div>
				</div>
			</div>
		</div>
		<br>
		<p class="lead">And I'm currently taking the following units to further my knowledge</p>
		<div class="container">
			<div class="row">
				<div class="col-sm-6">
					<div id="accordion3">
						<div class="card">
						  <div class="card-header " id="Semester3">
							<h5 class="mb-0">
							  <button class="btn btn-link collapsed" data-toggle="collapse" data-target="#collapseThree" aria-expanded="false" aria-controls="collapseThree">
								Semester 3
							  </button>
							</h5>
						  </div>
						  <div id="collapseThree" class="collapse " aria-labelledby="Semester3" data-parent="#accordion3">
							<div class="card-body">
								<ul class=" list-group list-group-flush">
									<li class="list-group-item "><strong>-COS20019</strong> Cloud Computing Architecture</li>
									<li class="list-group-item "><strong>-COS30008</strong> Data Structures and Patterns</li>
									<li class="list-group-item "><strong>-COS30011</strong> IoT Programming</li>
									<li class="list-group-item "><strong>-COS30019</strong> Introduction to Artificial Intelligence</li>
								</ul>
							</div>
						  </div>
						</div>
					</div>
				</div>
				<br>
				<div class="col-sm-6">
					<div id="accordion4">
						<div class="card">
						  <div class="card-header " id="Semester4">
							<h5 class="mb-0">
							  <button class="btn btn-link collapsed" data-toggle="collapse" data-target="#collapseFour" aria-expanded="false" aria-controls="collapseFour">
								Semester 4
							  </button>
							</h5>
						  </div>
						  <div id="collapseFour" class="collapse " aria-labelledby="Semester4" data-parent="#accordion4">
							<div class="card-body">
								<ul class=" list-group list-group-flush">
									<li class="list-group-item "><strong>-COS30017</strong> Software Development for Mobile Devices</li>
									<li class="list-group-item "><strong>-COS30023</strong> Languages in Software Development</li>
									<li class="list-group-item "><strong>-SWE20001</strong> Managing Software Projects</li>
									<li class="list-group-item "><strong>-SWE30009</strong> Software Testing and Reliability</li>
								</ul>
							</div>
						  </div>
						</div>
					</div>
				</div>
			</div>
		</div>
		<br>
		<p class="lead">I have knowledge on the following languages and tools</p>
		<div class="container">
			<div class="row">
				<div class="col-sm-6">
					<div id="accordion5">
						<div class="card">
						  <div class="card-header " id="language">
							<h5 class="mb-0">
							  <button class="btn btn-link collapsed" data-toggle="collapse" data-target="#collapseFive" aria-expanded="false" aria-controls="collapseFive">
								Languages
							  </button>
							</h5>
						  </div>
							  <div id="collapseFive" class="collapse " aria-labelledby="language" data-parent="#accordion5">
								<div class="card-body">
									<ul class=" list-group list-group-flush">
										<li class="list-group-item "><strong>-*HTML5</strong> <em>(Markup language)</em></li>
										<li class="list-group-item "><strong>-*CSS3</strong> <em>(Style language)</em></li>
										<li class="list-group-item "><strong>-Javascript</strong></li>
										<li class="list-group-item "><strong>-PHP</strong></li>
										<li class="list-group-item "><strong>-C#</strong></li>
										<li class="list-group-item "><strong>-Ruby</strong></li>
										<li class="list-group-item "><strong>-MySQL</strong></li>
									</ul>
								</div>
							  </div>
						</div>
					</div>
				</div>
				<br>
				<div class="col-sm-6">
					<div id="accordion6">
						<div class="card">
							  <div class="card-header " id="Tools">
								<h5 class="mb-0">
								  <button class="btn btn-link collapsed" data-toggle="collapse" data-target="#collapseSix" aria-expanded="false" aria-controls="collapseSix">
									Tools
								  </button>
								</h5>
							  </div>
							  <div id="collapseSix" class="collapse " aria-labelledby="Tools" data-parent="#accordion6">
								<div class="card-body">
									<ul class=" list-group list-group-flush">
										<li class="list-group-item "><strong>-Visual Studio Code</strong></li>
										<li class="list-group-item "><strong>-PHP My Admin</strong></li>
										<li class="list-group-item "><strong>-Adobe Photoshop</strong></li>
										<li class="list-group-item "><strong>-Adobe XD</strong></li>
										<li class="list-group-item "><strong>-Adobe Illustrator</strong></li>
										<li class="list-group-item "><strong>-Node.js</strong></li>
									</ul>
								</div>
							  </div>
						</div>
					</div>
				</div>
			</div>
		</div>
	</div>
</div>

<style>
	.content {
		width: 100%;
		max-width: var(--column-width);
		margin: var(--column-margin-top) auto 0 auto;
	}
</style>
