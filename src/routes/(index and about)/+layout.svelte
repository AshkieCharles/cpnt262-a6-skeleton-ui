<script>
  import '../../app.postcss';
	import { AppShell, AppBar, LightSwitch } from '@skeletonlabs/skeleton';
</script>


<AppShell>
	<svelte:fragment slot="header">
		<!-- App Bar -->
		<AppBar
			slotDefault="place-self-center"
			slotTrail="place-content-end"
			background="bg-secondary-50-900-token"
		>
			<a
				class="btn btn-sm variant-ghost-surface"
				href="../"
				rel="noreferrer"
			>
				Home
			</a>
			<a
				class="btn btn-sm variant-ghost-surface"
				href="../about"
				rel="noreferrer"
			>
				About
			</a>
			<a
				class="btn btn-sm variant-ghost-surface"
				href="../gallery"
				rel="noreferrer"
			>
				Gallery
			</a>
			<svelte:fragment slot="trail">
				<LightSwitch />
			</svelte:fragment>
		</AppBar>
		
	</svelte:fragment>

	
  <slot />
	<svelte:fragment slot="pageFooter">
		<footer class="bg-primary-500 text-center">&copy; Ashkie Esperanza 2023</footer></svelte:fragment>
</AppShell>

