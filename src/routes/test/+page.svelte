<script>
	const l = Array(100).fill(0);
</script>

<div class="g">
	{#each l as _}
		<button class="l{_}" on:click={() => (_ = _ == 1 ? 0 : 1)}></button>
	{/each}
</div>

<style>
	.g {
		display: grid;
		grid-template-columns: repeat(10, 1fr);
	}
	.g button {
		padding: 10px;
		border: 1px solid black;
		text-align: center;
		cursor: pointer;
	}
	.g button.l0 {
		background-color: antiquewhite;
	}
	.g button.l1 {
		background-color: rgb(167, 214, 200);
	}
</style>
