<script>
	/* import Counter from './Counter.svelte'; */
	/* import welcome from '$lib/images/svelte-welcome.webp'; */
	/* import welcome_fallback from '$lib/images/svelte-welcome.png'; */

  import video from '$lib/videos/1080.mp4';
</script>

<svelte:head>
	<title>Home</title>
	<meta name="description" content="Svelte demo app" />
</svelte:head>

<video id="background-video" autoplay loop muted>
  <source src={video} type="video/mp4">
</video>

<!-- <section> -->
<!-- 	<h1> -->
<!-- 		<span class="welcome"> -->
<!-- 			<picture> -->
<!-- 				<source srcset={welcome} type="image/webp" /> -->
<!-- 				<img src={welcome_fallback} alt="Welcome" /> -->
<!-- 			</picture> -->
<!-- 		</span> -->
<!---->
<!-- 		to your new<br />SvelteKit app -->
<!-- 	</h1> -->
<!---->
<!-- 	<h2> -->
<!-- 		try editing <strong>src/routes/+page.svelte</strong> -->
<!-- 	</h2> -->
<!---->
<!-- 	<Counter /> -->
<!-- </section> -->

<style>
  video {
    width: 100%;
    height: 100%;
    object-fit: cover;
  }

	/* section { */
	/* 	display: flex; */
	/* 	flex-direction: column; */
	/* 	justify-content: center; */
	/* 	align-items: center; */
	/* 	flex: 0.6; */
	/* } */

	/* h1 { */
	/* 	width: 100%; */
	/* } */

	/* .welcome { */
	/* 	display: block; */
	/* 	position: relative; */
	/* 	width: 100%; */
	/* 	height: 0; */
	/* 	padding: 0 0 calc(100% * 495 / 2048) 0; */
	/* } */

	/* .welcome img { */
	/* 	position: absolute; */
	/* 	width: 100%; */
	/* 	height: 100%; */
	/* 	top: 0; */
	/* 	display: block; */
	/* } */
</style>
