<script>
	import { push } from 'svelte-spa-router';
</script>

<button type="button"
	on:click={() => push('/date')}>
	Go To Date
</button>

<button type="button"
	on:click={() => push('/date/invalid')}>
	Go To Date (Error)
</button>
