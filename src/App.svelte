<script>
	import Router from 'svelte-spa-router';
	import Home from './router/Home.svelte';
	import About from './router/About.svelte';
	import Notice from './router/Notice.svelte';
	import QnA from './router/QnA.svelte';
	import NotFound from './router/NotFound.svelte';

	const routes = {
		'/':Home,
		'/About':About,
		'/Notice':Notice,
		'/QnA':QnA,

		'*':NotFound
	};
</script>

<nav>
	<a href="#/">Home</a>
	<a href="#/About">About</a>
	<a href="#/Notice">Notice</a>
	<a href="#/QnA">QnA</a>
</nav>

<Router {routes} />
