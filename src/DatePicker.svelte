<script>
	import { DatePicker, DatePickerInput } from 'carbon-components-svelte';
	import { replace } from 'svelte-spa-router';

	export let params = {};

	let value = '01/01/2000';

	$: if (params.value == 'invalid')
		replace('/')
</script>

<DatePicker datePickerType="single" bind:value={value}>
	<DatePickerInput labelText="Date"/>
</DatePicker>
