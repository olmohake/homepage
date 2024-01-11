<script>
	// Your selected Skeleton theme:
	import '@skeletonlabs/skeleton/themes/theme-skeleton.css';
	// This contains the bulk of Skeletons required styles:
	import '@skeletonlabs/skeleton/styles/skeleton.css';
	// Finally, your application's global stylesheet (sometimes labeled 'app.css')

	import hljs from 'highlight.js';
	import 'highlight.js/styles/github-dark.css';
	import '../app.css';
	import { storeHighlightJs } from '@skeletonlabs/skeleton';
	storeHighlightJs.set(hljs);
	import { AppShell, AppBar, LightSwitch } from '@skeletonlabs/skeleton';
	import { Modal } from '@skeletonlabs/skeleton';
	import { modalComponentRegistry } from './modalComponents';
</script>

<Modal components={modalComponentRegistry} />
<AppShell>
	<svelte:fragment slot="header">
		<!--AppBar>
			<svelte:fragment slot="lead"><h3 class="h3">Olmo Hake</h3></svelte:fragment>

			<svelte:fragment slot="trail">
				<a href="/key.asc" type="button" class="btn btn-sm variant-filled-surface">
					<Icon icon="ph:key-fill" class="inline text-warning-500 text-lg" />
					<span class="ml-1">PGP</span>
				</a>
				<LightSwitch />
			</svelte:fragment>
		</AppBar-->
	</svelte:fragment>
	<slot />
</AppShell>

<style>
</style>
