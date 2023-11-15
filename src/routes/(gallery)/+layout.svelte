<script>
	import '../../app.postcss';
	import { AppShell, AppBar, LightSwitch } from '@skeletonlabs/skeleton';
</script>

<header class="bg-black p-4 " >
	<AppShell class="text-gray-950">
		<!-- App Bar -->
		<AppBar
			slotTrail="place-content-start"
			background="bg-secondary-900-50-token"
		>
			<a
				class="btn btn-sm variant-glass-surface dark:md:hover:bg-fuchsia-600"
				href="../"
				rel="noreferrer"
			>
				Home
			</a>
			<a
				class="btn btn-sm variant-glass-surface dark:md:hover:bg-fuchsia-600"
				href="../about"
				rel="noreferrer"
			>
				About
			</a>
			<a
				class="btn btn-sm variant-glass-surface dark:md:hover:bg-fuchsia-600"
				href="../gallery"
				rel="noreferrer"
			>
				Gallery
			</a>
			<svelte:fragment slot="trail">
				<LightSwitch />
			</svelte:fragment>
		</AppBar>
		</AppShell>
	</header>
	<AppShell>
	<slot />
	<svelte:fragment slot="pageFooter">&copy; Ashkie Esperanza 2023</svelte:fragment>
</AppShell>







