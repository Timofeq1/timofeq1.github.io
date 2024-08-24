<script>
	let time = 0;
</script>

<main>
	<div class="video-wrapper">
		<video class="video-background" autoplay muted loop>
			<source src="/bg1.mp4" type="video/mp4" />
			Your browser does not support the video tag.
		</video>
	</div>
	<div class="content">
		<h1>Under development...</h1>
		<p>Sorry, this page is currently under development</p>
		<li><a href="/">Go to main page</li>
	</div>
</main>

<style>
	main {
		position: relative;
		overflow: hidden;
		width: 100%;
		height: 100vh;
	}

	.video-wrapper {
		position: fixed;
		top: 0;
		left: 0;
		width: 100%;
		height: 100%;
		overflow: hidden;
	}

	.video-background {
		position: absolute;
		top: 0;
		left: 0;
		width: 100%;
		height: 100%;
		object-fit: cover;
		filter: blur(1px); /* Add blur effect */
	}

	/* Create an overlay to cover the blurred borders */
	.video-wrapper::before {
		content: '';
		position: absolute;
		top: 0;
		left: 0;
		width: 100%;
		height: 100%;
		box-shadow: inset 0 0 0 5vw rgba(0, 0, 0, 10); /* Adjust the shadow to cover the blurred edges */
		pointer-events: none;
	}

	.content {
		position: relative;
		z-index: 1;
		color: white;
		text-align: center;
		padding: 2rem;
		background: rgba(0, 0, 0, 0.6); /* Modify the background color and opacity */
		border-radius: 3px; /* Add rounded corners */
		max-width: 600px; /* Center content */
		margin: 20% auto; /* Center content vertically and horizontally */
	}

</style>
