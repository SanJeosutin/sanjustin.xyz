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
				<h1 class="display-5">Send me an email 😊</h1>
			</div>
			<div class="card-body">
				<div class="lead">
					<form id="contactMe" method="POST" action="">
                        <div class="form-group">
                            <label for="name">Name</label>
                            <div class="input-group">
                                <input id="name" name="name" placeholder="John Smith" type="text" aria-describedby="nameHelpBlock" required="required" class="form-control">
                            </div>
                        </div>
                        <br>
                        <div class="form-group">
                            <label for="email">Email</label>
                            <div class="input-group">
                                <input id="email" name="email" placeholder="johnsmith@example.com" type="text" aria-describedby="emailHelpBlock" required="required" class="form-control">
                            </div>
                        </div>
                        <br>
                        <div class="form-group">
                            <label for="subject">Subject</label>
                            <div>
                                <select id="subject" name="subject" aria-describedby="subjectHelpBlock" required="required" class="form-select-sm">
                                    <option value="work">Potential Work</option>
                                    <option value="projectDiscussion">Project Discussion</option>
                                    <option value="feedback">Feedback</option>
                                    <option value="other">Other</option>
                                </select>
                            </div>
                        </div>
                        <br>
                        <div class="form-group">
                            <label for="message">Message</label>
                            <textarea id="message" name="message" cols="40" rows="5" required="required" class="form-control"></textarea>
                        </div>
                        <br>
                        <div class="form-group">
                            <button name="submit" type="submit" class="btn btn-dark"><i class="fa fa-paper-plane"></i>{@html '&ThickSpace;'}Send it!</button>
                        </div>
                    </form>
				</div>
			</div>
		</div>
	</div>
</div>