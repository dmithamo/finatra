<script>
	import AppFooter from '$lib/components/app-footer.svelte';
	import AppLogo from '$lib/components/app-logo.svelte';
</script>

<div class="flex h-full flex-col items-center justify-center gap-1 p-6">
	<h1 class="text-2xl font-bold">Welcome to{' '}<AppLogo isNameOnly={true} />!</h1>
	<p class="text-center text-sm">
		Your privacy-preserving financial health companion (with AI&trade; and stuff)
	</p>
</div>
<AppFooter />
