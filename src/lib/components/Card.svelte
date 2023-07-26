<script lang="ts">
  import Icon from "@iconify/svelte";

  export let title = "ilovecoffee";
  export let description = "A RESTful API created via Nest.js";
  export let tags: string[] = ["nestjs", "javascript"];
  export let url = "";
</script>

<div
  class="flex flex-col max-w-xs p-5 gap-4 bg-white text-black rounded-md transition duration-300 ease-out lg:hover:scale-110"
>
  <h2 class="text-2xl font-bold">{title}</h2>
  <p class="text-sm font-light">{description}</p>
  <div class="flex items-center">
    <div class="flex gap-3 flex-wrap">
      {#each tags as tag}
        <span>#{tag}</span>
      {/each}
    </div>
    <a
      class="no-underline decoration-inherit ml-auto mr-3"
      href={url}
      target="_blank"
    >
      <Icon icon="mdi:github" width="30" />
    </a>
  </div>
</div>
