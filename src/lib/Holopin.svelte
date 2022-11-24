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
	<img src="https://holopin.me/{user}" alt="@{user}'s Holopin board" style="width: 100%" />
</a>
