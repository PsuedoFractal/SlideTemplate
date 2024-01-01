<script lang="ts">
    export let name = "source.md";
    export let external = false;
</script>

{#if external}
    <section 
    data-markdown={name}
    data-separator="\n---\n"
    data-separator-vertical="\n--\n"
    data-separator-notes="Note:"
    data-charset="utf-8"></section>
{:else}
    <section data-markdown>
        <div data-template>
            <slot />
        </div>
    </section>
{/if}