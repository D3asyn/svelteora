<script>
	var a = 0;
	var b = 0;
</script>

<h1>Eredmeny jelzo</h1>

<div>
	<a href="/svelteora/test">Animation</a>
</div>

<table>
	<tr>
		<th>A</th>
		<th>-</th>
		<th>B</th>
	</tr>
	<tr>
		<td>{a}</td>
		<td>-</td>
		<td>{b}</td>
	</tr>
	<tr>
		<td colspan="3">
			<button on:click={() => a++}>A noveles</button>
			<button on:click={() => b++}>B noveles</button>
		</td>
	</tr>
	<tr>
		<td colspan="3">
			<button on:click={() => a--}>A csokkentes</button>
			<button on:click={() => b--}>B csokkentes</button>
		</td>
	</tr>
</table>

<style>
	td {
		text-align: center;
	}
</style>
