<script lang="ts">
	import './layout.css';
	import favicon from '$lib/assets/favicon.svg';
	import { ModeWatcher } from 'mode-watcher';
	import * as Sidebar from '$lib/components/ui/sidebar/index';
	import AppSidebar from '$lib/components/app-sidebar.svelte';
	import AppThemeToggler from '$lib/components/app-theme-toggler.svelte';
	let { children } = $props();
</script>

<svelte:head><link rel="icon" href={favicon} /></svelte:head>

<ModeWatcher />

<Sidebar.Provider>
	<AppSidebar />
	<main class="flex h-screen w-full flex-col">
		<header class="flex h-16 w-full items-center justify-end gap-2 border-b px-4">
			<AppThemeToggler />
		</header>
		<section class="flex-1">
			{@render children()}
		</section>
	</main>
</Sidebar.Provider>
