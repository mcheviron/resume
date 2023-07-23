<script lang="ts">
  import { page } from "$app/stores";
  import koala from "$lib/assets/koala.png";

  // isActive is not reactive by default so $: has to be used
  $: isActive = (url: string) => url === $page.url.pathname;
</script>

<nav>
  <a href="/" class="logo" class:active={isActive("/")}>Mostafa Cheviron</a>
  <ul>
    <li><a href="/about" class:active={isActive("/about")}>About</a></li>
    <li><a href="/skills" class:active={isActive("/skills")}>Skills</a></li>
    <li>
      <a href="/projects" class:active={isActive("/projects")}>Projects</a>
    </li>
  </ul>
  <div class="koala-container">
    <svg height="56" width="56" viewBox="0 0 56 56"
      ><path
        d="M29.465,0.038373A28,28,0,0,1,52.948,40.712L51.166,39.804A26,26,0,0,0,29.361,2.0356Z"
        class="yellow"
        fill="currentColor"
      /><path
        d="M51.483,43.250A28,28,0,0,1,4.5172,43.250L6.1946,42.161A26,26,0,0,0,49.805,42.161Z"
        class="blue"
        fill="currentColor"
      /><path
        d="M3.0518,40.712A28,28,0,0,1,26.535,0.038373L26.639,2.0356A26,26,0,0,0,4.8338,39.804Z"
        class="red"
        fill="currentColor"
      />
    </svg>
    <img src={koala} alt="koala" />
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
  nav {
    display: flex;
    align-items: center;
    gap: 4rem;
    margin-bottom: 3.5rem;
  }
  .logo {
    margin-right: auto;
    font-family: "Playfair Display", serif;
    font-size: 1.875rem;
  }
  .active::before {
    content: "";
    position: absolute;
    border-bottom: 2px solid white;
    width: 100%;
    bottom: -0.1875rem;
  }
  ul {
    display: flex;
    gap: 3.8125rem;
    justify-content: flex-end;
    align-items: center;
  }
  li {
    list-style-type: none;
  }
  a {
    text-decoration: none;
    color: white;
    font-size: 1.125rem;
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
  .koala-container {
    position: relative;
    display: flex;
    align-items: center;
    justify-content: center;
    width: 56px;
    height: 56px;
  }

  .koala-container img {
    width: 80%;
    height: 80%;
    border-radius: 50%;
  }

  .koala-container svg {
    position: absolute;
    top: 0;
    left: 0;
    animation: spin 4s linear infinite;
  }
  .koala-container:hover svg {
    animation: spinReverse 2s linear infinite;
  }

  @keyframes spin {
    0% {
      transform: rotate(0deg);
    }
    100% {
      transform: rotate(360deg);
    }
  }

  @keyframes spinReverse {
    0% {
      transform: rotate(0deg);
    }
    100% {
      transform: rotate(-360deg);
    }
  }
  .yellow {
    fill: #ffd644;
  }
  .blue {
    fill: #36a3ff;
  }
  .red {
    fill: #ff4545;
  }
</style>
