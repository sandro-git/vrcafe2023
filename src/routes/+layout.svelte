<script lang="ts">
	// The ordering of these imports is critical to your app working properly
	import '@skeletonlabs/skeleton/themes/theme-modern.css';
	// If you have source.organizeImports set to true in VSCode, then it will auto change this ordering
	import '@skeletonlabs/skeleton/styles/skeleton.css';
	// Most of your app wide CSS should be put in this file
	import '../app.postcss';
	import { AppShell, AppBar } from '@skeletonlabs/skeleton';
	import Footer from '$lib/components/Footer.svelte';
</script>

<AppShell>
	<!-- <svelte:fragment slot="header">
		<AppBar
			gridColumns="grid-cols-3"
			slotLead="place-content-start"
			slotDefault="place-self-center"
			slotTrail="place-content-end"
			border="border-b-2"
		>
			<svelte:fragment slot="lead">
				<img class="w-96 md:w-1/3" src="logo.png" alt="logo" />
			</svelte:fragment>
			<svelte:fragment slot="default">
				<h1 class="h1 hidden md:block">Réalité Virtuelle</h1>
			</svelte:fragment>
			<svelte:fragment slot="trail">
				<button class="btn btn-lg variant-filled-primary">Réserver</button>
			</svelte:fragment>
		</AppBar>
	</svelte:fragment> -->
	<!-- (sidebarLeft) -->
	<!-- (sidebarRight) -->
	<!-- (pageHeader) -->
	<!-- Router Slot -->
	<slot />
	<!-- ---- / ---- -->
	<!-- <svelte:fragment slot="footer"><Footer /></svelte:fragment> -->
	<!-- (footer) -->
</AppShell>
