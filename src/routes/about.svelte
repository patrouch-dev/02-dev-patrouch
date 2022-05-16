<script>
	import Icon from './Icon.svelte';
	import Nested from './Nested.svelte';
	let string = `this string contains some <strong>HTML!!!</strong>`;

	let count = 0;

	function incrementCount() {
		count += 1;
	}
</script>

<svelte:head>
	<title>About</title>

	<style>
		@import url('https://fonts.googleapis.com/css2?family=Marmelad&family=Pacifico&family=Special+Elite&family=Tangerine:wght@400;700&family=Ultra&display=swap');
		h1 {
			font-family: 'Special Elite', cursive;
		}

		p {
			font-family: 'Marmelad', sans-serif;
			color: purple;
		}

		body {
			background-color: #af875f;
		}
	</style>
</svelte:head>
<h1 class="text-3xl font-bold">about patrouch.dev</h1>

<button on:click={incrementCount}>
	Clicked {count}
	{count === 1 ? 'time' : 'times'}
</button>
<Icon name="trash" class="this-is-optional" />

<p>{@html string}</p>
<Nested />
<svg
	class="h-6 w-6 text-gray-500, fill-cyan-500 hover:stroke-cyan-700"
	fill="none"
	viewBox="0 0 24 24"
	stroke="currentColor"
	stroke-width="2"
>
	<path
		stroke-linecap="round"
		stroke-linejoin="round"
		d="M12 8v4l3 3m6-3a9 9 0 11-18 0 9 9 0 0118 0z"
	/>
</svg>

<p>
	This website is built with Sveltekit. It is served from an off-premise virtual server (Ubuntu) on
	Google Compute Engine. Nginx is configured for these purposes as a reverse proxy with an upstream
	directive. Other technologies used for this website are Node, PM2, and Letsencrypt. The DNS is
	managed through Google Domains. The local development machine is an HP Chromebook (8GB ram, 64GB
	storage, Intel M3 -- with GNU/Linux enabled. This website uses Google Analytics and possibly other
	tracking software and for that reason (and certainly many more reasons) this site is not compliant
	with basic user freedoms the way it ought be. For more information on technology's destruction of
	your freedom, start here: <a href="http://fsf.org">Free Software Movement</a>
</p>

<style>
	h1 {
		font-family: 'Special Elite', cursive;
	}
	p {
		font-family: 'Marmelad', sans-serif;
		color: black;
		font-size: 2em;
	}
</style>
