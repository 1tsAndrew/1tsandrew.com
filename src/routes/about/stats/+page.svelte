<script>
	import Header from "../Header.svelte";

let visits

	if (typeof localStorage == "object") {
		visits = localStorage.getItem("visits")
	}
</script>

<svelte:head>
	<meta charset="utf-8" />
	<meta name="viewport" content="width=device-width, initial-scale=1" />
	<title>Andrew's World!</title>

	<meta property="og:title" content="Andrew's World" />
	<meta property="og:site_name" content="penis.today" />
	<meta property="og:url" content="https://penis.today" />
	<meta property="og:description" content="AIOA (All in one Andrew)" />
	<meta property="og:type" content="website" />
	<meta
		property="og:image"
		content="https://cdn.discordapp.com/avatars/355091763825868800/a_aede142fc5586b648e038486987f4090.gif?size=1024"
	/>
</svelte:head>

<Header />

<h2>My website has <strong>{visits | ""}</strong> visits!</h2>

<table role="grid">
	<thead
		><tr
			><th scope="col">#</th> <th scope="col">Use</th>
			<th scope="col">CPU</th> <th scope="col">GPU</th>
			<th scope="col">Memory</th> <th scope="col">Storage</th></tr
		></thead
	>
	<tbody
		><tr
			><th scope="row">Main Laptop</th> <td>Everything</td>
			<td>11th Gen Intel(R) Core(TM) i7-11800H @ 2.30GHz</td>
			<td>NVIDIA GeForce RTX 3070</td> <td>15258 MiB</td>
			<td>1 TB SSD</td></tr
		>
		<tr
			><th scope="row">2nd Laptop</th> <td>School<br>Work</td>
			<td>12th Gen Intel(R) Core(TM) i5-1235U @ 1.30 GHz</td>
			<td>Integrated Intel Iris XE</td> <td>22888 MiB</td>
			<td>512 GB SSD </td></tr
		>
	</tbody>
</table>
