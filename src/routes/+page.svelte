<script>
	import { onMount } from 'svelte';
	import { themeChange } from 'theme-change';

	// NOTE: the element that is using one of the theme attributes must be in the DOM on mount
	onMount(() => {
		themeChange(false);
		// 👆 false parameter is required for svelte
	});
</script>

<button class="btn">Some Text</button>

<select data-choose-theme>
	<option value="light">Light</option>
	<option value="dark">Dark</option>
	<option value="black">Black</option>
</select>
