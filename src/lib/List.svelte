<script>
	const listItems = [
		{ name: 'Bethesda' },
		{ name: 'Larian'},
		{ name: 'Bungie' },
    { name: 'BioWare'},
    { name: "Ubisoft"}
	];
</script>


<h2 class="text-center my-10"> Famous Game Studios</h2>
	<ul class="text-center">
		{#each listItems as {name}}
			<li>{name}</li>
		{/each}
	</ul>

