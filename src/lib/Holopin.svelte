<script lang="ts">
	/** The [Holopin](https://holopin.io/) user. */
	export let user: string;
</script>

<!--
	@component
	An image of the desired user's [Holopin](https://holopin.io/) badges, which is a link to view their full Holopin profile (100% width)

	Usage:

	```tsx
	<Holopin user="zaneshaw">
	```
-->
<a href="https://holopin.io/@{user}">
	<img src="https://holopin.me/{user}" alt="An image of @{user}'s Holopin badges, which is a link to view their full Holopin profile" />
</a>

<style>
	img {
		width: 100%;
		border-radius: 0.75rem;
		cursor: pointer;
		filter: grayscale(50%);
		transition-duration: 200ms;
	}

	img:hover {
		filter: grayscale(0%);
	}
</style>
