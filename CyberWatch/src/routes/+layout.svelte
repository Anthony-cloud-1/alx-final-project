<script lang="ts">
	import './styles.css';
	import * as Resizable from '$lib/components/ui/resizable';
	import { ModeWatcher } from 'mode-watcher';
	import Analysis from '$lib/components/analysis.svelte';
</script>

<ModeWatcher />
<main class="h-screen p-4">
	<Resizable.PaneGroup direction="horizontal" class="!h-full rounded-lg border">
		<Resizable.Pane>
			<slot></slot>
		</Resizable.Pane>
		<Resizable.Handle class="hidden sm:block"/>
		<Resizable.Pane class="hidden sm:flex flex-col h-full overflow-y-scroll">
			<div class="flex-1 overflow-y-auto">
				<Analysis />
			</div>
		</Resizable.Pane>
	</Resizable.PaneGroup>
</main>
