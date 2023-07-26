<script lang="ts">
  import { page } from "$app/stores";
  import koala from "$lib/assets/koala.png";

  // isActive is not reactive by default so $: has to be used
  $: isActive = (url: string) => url === $page.url.pathname;
</script>

<nav class="flex items-center mx-3.5 gap-16 mb-14 md:mx-10 lg:max-w-6xl">
  <a
    href="/"
    class="md:mr-auto font-['Playfair_Display'] text-3xl"
    class:active={isActive("/")}
  >
    Mostafa Cheviron
  </a>
  <ul class="md:flex gap-16 justify-end items-center hidden">
    <li>
      <a class="text-lg" href="/about" class:active={isActive("/about")}
        >About</a
      >
    </li>
    <li>
      <a class="text-lg" href="/skills" class:active={isActive("/skills")}
        >Skills</a
      >
    </li>
    <li>
      <a class="text-lg" href="/projects" class:active={isActive("/projects")}
        >Projects
      </a>
    </li>
  </ul>
  <div class="hidden relative lg:flex items-center justify-center w-14 h-14">
    <svg
      class="absolute top-0 left-0 animate-spin-slow hover:animate-spin-reverse"
      height="56"
      width="56"
      viewBox="0 0 56 56"
      ><path
        d="M29.465,0.038373A28,28,0,0,1,52.948,40.712L51.166,39.804A26,26,0,0,0,29.361,2.0356Z"
        class="fill-[#ffd644]"
        fill="currentColor"
      /><path
        d="M51.483,43.250A28,28,0,0,1,4.5172,43.250L6.1946,42.161A26,26,0,0,0,49.805,42.161Z"
        class="fill-[#36a3ff]"
        fill="currentColor"
      /><path
        d="M3.0518,40.712A28,28,0,0,1,26.535,0.038373L26.639,2.0356A26,26,0,0,0,4.8338,39.804Z"
        class="fill-[#ff4545]"
        fill="currentColor"
      />
    </svg>
    <img src={koala} alt="koala" class="w-3/4 h-3/4 rounded-full" />
  </div>
</nav>

<style>
  :global(*) {
    box-sizing: border-box;
    margin: 0;
  }
  :global(body) {
    background-color: #1f2028;
    color: white;
    font-family: "Roboto", sans-serif;
    max-width: 75rem;
    margin: 0 auto;
    padding-top: 3.125rem;
  }
  .active::before {
    content: "";
    position: absolute;
    border-bottom: 2px solid white;
    width: 100%;
    bottom: -0.1875rem;
  }

  li {
    list-style-type: none;
  }
  a {
    text-decoration: none;
    color: white;
    position: relative;
  }
  a::before {
    content: "";
    position: absolute;
    border-bottom: 0.125rem solid white;
    width: 0%;
    bottom: -0.1875rem;
    transition: 0.3s;
  }
  a:not(.active):hover:before {
    width: 100%;
  }
</style>
