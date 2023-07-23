<script>
  import Navbar from "$lib/components/Navbar.svelte";
  import { fly } from "svelte/transition";
  import { page } from "$app/stores";

  $: path = $page.url.pathname.slice(1)
    ? $page.url.pathname.charAt(1).toUpperCase() + $page.url.pathname.slice(2)
    : "Home";
</script>

<svelte:head>
  <title>{path}</title>
</svelte:head>
<Navbar />
{#key $page.url}
  <div in:fly={{ x: "-100%", duration: 1000 }}>
    <slot />
  </div>
{/key}
