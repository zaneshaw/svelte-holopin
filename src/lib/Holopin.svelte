<script lang="ts">
	/** The [Holopin](https://holopin.io/) user. */
	export let user: string;
</script>

<!--
	@component
	Displays the desired user's [Holopin](https://holopin.io/) board (100% width).

	Usage:

	```tsx
	<Holopin user="zaneshaw">
	```
-->
<a href="https://holopin.io/@{user}">
	<img src="https://holopin.me/{user}" alt="@{user}'s Holopin board" />
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
