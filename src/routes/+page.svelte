<script>
	import AppLogo from '$lib/components/app-logo.svelte';
</script>

<div class="flex h-full flex-col items-center justify-center">
	<h1 class="text-4xl font-bold">Welcome to{' '}<AppLogo isNameOnly={true} />!</h1>
	<p>Your privacy-preserving financial health companion (with AI&trade; and stuff)</p>
</div>
<footer class="flex h-24 w-full items-center justify-center gap-4 border-t px-4 text-xs">
	<AppLogo />
	<span class="opacity-75"
		>Designed and developed by {' '}<a
			class="underline underline-offset-3"
			href="https://github.com/dmithamo"
			target="_blank"
			rel="norefferer">D Mithamo</a
		></span
	>
</footer>
