<script>
	import Home from './Home.svelte';
	import DatePicker from './DatePicker.svelte';
	import Router from 'svelte-spa-router';

	const routes = {
		'/': Home,
		'/date/:value?': DatePicker,
	};
</script>

<svelte:head>
	<link rel="stylesheet" href="https://unpkg.com/carbon-components-svelte/css/g100.css" />
</svelte:head>

<Router {routes} />
