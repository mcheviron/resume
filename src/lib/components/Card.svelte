<script lang="ts">
  import Icon from "@iconify/svelte";

  export let title = "ilovecoffee";
  export let description = "A RESTful API created via Nest.js";
  export let tags: string[] = ["nestjs", "javascript"];
  export let url = "";
</script>

<div class="card">
  <h2>{title}</h2>
  <p>{description}</p>
  <div class="bottom">
    <div class="tags">
      {#each tags as tag}
        <span>#{tag}</span>
      {/each}
    </div>
    <a href={url} class="github" target="_blank">
      <Icon icon="mdi:github" width="30" />
    </a>
  </div>
</div>

<style>
  .card {
    display: flex;
    flex-direction: column;
    max-width: 20rem;
    padding: 1.25rem;
    gap: 0.9375rem;
    background-color: white;
    color: black;
    border-radius: 5px;
    transition: 0.3s ease-out;
  }
  .card:hover {
    transform: scale(1.1);
  }
  .bottom {
    display: flex;
    align-items: center;
  }
  .tags {
    display: flex;
    gap: 0.625rem;
    flex-wrap: wrap;
  }
  .github {
    margin-left: auto;
    margin-right: 10px;
  }
  h2 {
    font-size: 25px;
    font-weight: bold;
  }
  p {
    font-size: 16px;
    font-weight: lighter;
  }
  a {
    text-decoration: none;
    color: inherit;
  }
</style>
