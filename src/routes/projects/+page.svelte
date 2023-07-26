<script>
  import Card from "$lib/components/Card.svelte";
  import projects from "$lib/assets/projects.json";
</script>

<div class="grid grid-cols-3 place-content-center gap-7 my-8">
  {#each projects as project}
    <Card {...project} />
  {/each}
</div>
