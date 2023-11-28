<script>
	import flowers1 from '$lib/images/flowers_1.jpg';
	import flowers2 from '$lib/images/flowers_2.jpg';

	import Tidal from '$lib/images/Tidal.svelte';
</script>

<svelte:head>
	<title>About</title>
	<meta name="description" content="About this app" />
</svelte:head>

<div class="text-column">
	<h1>Links:</h1>

	<!-- <img src={flowers1} alt="Flowers image 1" /> -->

	<!-- <img src={flowers2} alt="Flowers image 2" /> -->

	<!-- TODO: rel="me nofollow ugc"  -->
	<a
		href="https://tidal.com/browse/track/326087341"
		target="_blank"
		rel="noopener noreferrer"
	>
		<Tidal />
	</a>
</div>
