<script>
	const listItems = [
		{ name: 'Bethesda', game: "Fallout", href: "https://en.wikipedia.org/wiki/Fallout_(series)" },
		{ name: 'Larian', game: "Baldur's Gate", href: "https://en.wikipedia.org/wiki/Baldur%27s_Gate"},
		{ name: 'Bungie', game: "Destiny", href: "https://en.wikipedia.org/wiki/Destiny_(video_game)" },
    { name: 'Miyoho', game: "Honkai Star Rail", href: "https://en.wikipedia.org/wiki/Honkai:_Star_Rail"},
    { name: "Ubisoft", game: "Rainbow Six Siege", href: "https://en.wikipedia.org/wiki/Tom_Clancy%27s_Rainbow_Six_Siege"}
	];
</script>


<h2 class="text-center my-10 font-token"> Famous Game Studios</h2>
	<ul class="text-center">
		{#each listItems as {name, game, href}}
      <!-- Design tokens wont work so I just used regular tailwind but with the colors of Skeleton UI-->
			<li class="border-token max-w-md flex m-auto "><a class="hover:bg-surface-500 text-primary-500" {href}>{name} made {game} and are popular because of this game.</a></li>
		{/each}
	</ul>

