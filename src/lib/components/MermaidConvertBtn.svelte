<script lang="ts">
    import IconConvert from "./icons/IconConvert.svelte";
    export let classNames = "";
    export let onToggle;
</script>

<button class={classNames} title={"Convert Mermaid Chart <-> Code"} type="button" on:click={onToggle} >
    <div class="relative">
		<slot>
			<IconConvert classNames="h-[1.14em] w-[1.14em]" />
		</slot>
	</div>
</button>
