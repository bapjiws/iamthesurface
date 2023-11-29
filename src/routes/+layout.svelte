<script>
	import { browser } from '$app/environment';
	import { page } from '$app/stores';
	import { webVitals } from '$lib/vitals';
	/* import Header from './Header.svelte'; */
	import './styles.css';

	import Bandcamp from '$lib/icons/Bandcamp.svelte';
	import Instagram from '$lib/icons/Instagram.svelte';
	import SoundCloud from '$lib/icons/SoundCloud.svelte';
	import Spotify from '$lib/icons/Spotify.svelte';
	import TikTok from '$lib/icons/TikTok.svelte';
	import YouTube from '$lib/icons/YouTube.svelte';

	/** @type {import('./$types').LayoutServerData} */
	export let data;

	$: if (browser && data?.analyticsId) {
		webVitals({
			path: $page.url.pathname,
			params: $page.params,
			analyticsId: data.analyticsId
		});
	}
</script>

<div class="app">
	<!-- <Header /> -->

	<main>
		<slot />
	</main>

	<footer>
		<a href="https://bapjiws.bandcamp.com" target="_blank" rel="noopener">
			<Bandcamp />
		</a>
		<a href="https://soundcloud.com/iamthesurface_iamthelion" target="_blank" rel="noopener">
			<SoundCloud />
		</a>
		<a href="https://open.spotify.com/track/6kYQstzc8ptJIIINlm6QSD" target="_blank" rel="noopener">
			<Spotify />
		</a>
		<a href="https://www.youtube.com/@iamthesurface_iamthelion" target="_blank" rel="noopener">
			<YouTube />
		</a>
		<a href="https://www.instagram.com/iamthesurface_official/" target="_blank" rel="noopener">
			<Instagram />
		</a><a href="https://www.tiktok.com/@iamthesurface_official" target="_blank" rel="noopener">
			<TikTok />
		</a>
	</footer>
</div>

<style>
	.app {
		display: flex;
		flex-direction: column;
    align-items: center;
		min-height: 100vh;
	}

	main {
		flex: 1;
		display: flex;
    height: 100%;
    flex-direction: column;
    justify-content: center;
		padding: 1rem;
		width: 100%;
		box-sizing: border-box;
	}

	footer {
		margin-top: auto;
		display: flex;
		/* flex-direction: column; */
		justify-content: center;
		align-items: center;
		padding: 24px;
    position: fixed;
    bottom: 0;
	}

	footer a {
		font-weight: bold;
		margin: 8px;
		height: 32px;
		width: 32px;
	}

	@media (min-width: 480px) {
		footer {
			padding: 24px 0;
		}
	}
</style>
