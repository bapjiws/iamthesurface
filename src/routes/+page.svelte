<script>
	/* import Counter from './Counter.svelte'; */
	/* import welcome from '$lib/images/svelte-welcome.webp'; */
	/* import welcome_fallback from '$lib/images/svelte-welcome.png'; */

	import cover from '$lib/images/cover.jpg';
	import sign from '$lib/images/sign.png';
  import video from '$lib/videos/1080.mp4';
</script>

<svelte:head>
	<title>Home</title>
	<meta name="description" content="Svelte demo app" />
</svelte:head>

<!-- <video id="background-video" autoplay muted> -->
<!--   <source src={video} type="video/mp4"> -->
<!-- </video> -->

<!-- <img src={sign} alt="Background" /> -->

<!-- <section> -->
<!--   <h1>Music</h1> -->
<!-- </section> -->

<div class="text-column">
	<!-- <h1>Ungive | Untake</h1> -->

	<article>
    Like mountains that ceased the above,<br>
    Like autumn reclaiming its leaves,<br>
    Untake from the ones that you love,<br>
    Ungive from your most precious deeds.
  </article>

</div>
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
  /* video { */
  /*   width: 100%; */
  /*   height: 100%; */
  /*   object-fit: cover; */
  /* } */

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
