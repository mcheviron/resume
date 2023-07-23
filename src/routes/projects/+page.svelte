<script>
  import Card from "$lib/components/Card.svelte";
  import projects from "$lib/assets/projects.json";
</script>

<div class="cards">
  {#each projects as project}
    <Card {...project} />
  {/each}
</div>

<style>
  .cards {
    display: flex;
    justify-content: center;
    align-items: center;
    flex-wrap: wrap;
    gap: 1.875rem;
  }
</style>
