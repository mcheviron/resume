<script>
  import Icon from "@iconify/svelte";
</script>

<div class="wrapper">
  <h1>
    I program in several languages, with different proficiencies. Ultimately, I
    don’t focus on the specific language too much and prefer to focus mainly on
    the implementation and language support. Not all languages are the same and
    if I am writing an OS, I wouldn’t use Typescript and if I am creating a
    frontend, I wouldn’t use Rust.
  </h1>
  <div class="button">
    <svg
      width="21"
      height="24"
      viewBox="0 0 21 24"
      fill="none"
      xmlns="http://www.w3.org/2000/svg"
    >
      <path
        d="M0.295607 14.33L9.95561 23.94L19.6156 14.33C19.7296 14.2432 19.8236 14.1329 19.8912 14.0067C19.9589 13.8804 19.9986 13.7411 20.0077 13.5981C20.0169 13.4551 19.9952 13.3119 19.9441 13.178C19.893 13.0442 19.8138 12.9228 19.7118 12.8223C19.6098 12.7217 19.4873 12.6442 19.3528 12.5951C19.2182 12.5459 19.0747 12.5263 18.9318 12.5375C18.789 12.5486 18.6503 12.5903 18.525 12.6598C18.3997 12.7292 18.2908 12.8248 18.2056 12.94L10.9556 20.13L10.9556 1C10.9556 0.734785 10.8503 0.480433 10.6627 0.292896C10.4752 0.10536 10.2208 1.90735e-06 9.95561 1.90735e-06C9.69039 1.90735e-06 9.43604 0.10536 9.2485 0.292896C9.06096 0.480433 8.95561 0.734785 8.95561 1L8.95561 20.13L1.70561 12.94C1.5173 12.753 1.26243 12.6485 0.99707 12.6494C0.731707 12.6504 0.477583 12.7567 0.290606 12.945C0.103628 13.1333 -0.000888824 13.3882 4.95911e-05 13.6535C0.000988007 13.9189 0.107304 14.173 0.295607 14.36V14.33Z"
        fill="white"
      />
    </svg>
  </div>
  <div class="lower-sec">
    <h2>
      The following tier list isn’t intended to reflect my objective knowledge
      of the languages, tools and frameworks, but how fast and how much I
      develop in them
    </h2>
    <div class="high">
      <p>High:</p>
      <div class="skills">
        <Icon
          class="icon"
          icon="teenyicons:javascript-outline"
          color="white"
          width="61"
          height="61"
        />
        <Icon
          class="icon"
          icon="fa6-brands:golang"
          color="white"
          width="61"
          height="61"
        />
        <Icon
          class="icon"
          icon="akar-icons:html-fill"
          color="white"
          width="61"
          height="61"
        />
        <Icon
          class="icon"
          icon="akar-icons:css-fill"
          color="white"
          width="61"
          height="61"
        />
        <Icon
          class="icon"
          icon="teenyicons:react-outline"
          color="white"
          width="61"
          height="61"
        />
        <Icon
          class="icon"
          icon="teenyicons:nextjs-solid"
          color="white"
          width="61"
          height="61"
        />
        <Icon
          class="icon"
          icon="teenyicons:nodejs-solid"
          color="white"
          width="61"
          height="61"
        />
        <Icon
          class="icon"
          icon="teenyicons:python-outline"
          color="white"
          width="61"
          height="61"
        />
        <Icon
          class="icon"
          icon="akar-icons:vscode-fill"
          color="white"
          width="61"
          height="61"
        />
        <Icon
          class="icon"
          icon="simple-icons:linux"
          color="white"
          width="61"
          height="61"
        />
        <Icon
          class="icon"
          icon="bi:windows"
          color="white"
          width="61"
          height="61"
        />
        <Icon class="icon" icon="bi:git" color="white" width="61" height="61" />
        <Icon
          class="icon"
          icon="bi:github"
          color="white"
          width="61"
          height="61"
        />
        <Icon
          class="icon"
          icon="file-icons:tailwind"
          color="white"
          width="61"
          height="61"
        />
        <Icon
          class="icon"
          icon="teenyicons:typescript-outline"
          color="white"
          width="61"
          height="61"
        />
        <Icon
          class="icon"
          icon="file-icons:svelte"
          color="white"
          width="61"
          height="61"
        />
      </div>
    </div>
    <div class="medium">
      <p>Medium:</p>
      <div class="skills">
        <Icon
          class="icon"
          icon="fa6-brands:docker"
          color="white"
          width="61"
          height="61"
        />
        <Icon
          class="icon"
          icon="mingcute:figma-line"
          color="white"
          width="61"
          height="61"
        />
        <Icon
          class="icon"
          icon="file-icons:nestjs"
          color="white"
          width="61"
          height="61"
        />
        <Icon
          class="icon"
          icon="simple-icons:csharp"
          color="white"
          width="61"
          height="61"
        />
        <Icon
          class="icon"
          icon="devicon-plain:java"
          color="white"
          width="61"
          height="61"
        />
      </div>
    </div>
    <div class="low">
      <p>Low:</p>
      <div class="skills">
        <Icon
          class="icon"
          icon="cib:rust"
          color="white"
          width="61"
          height="61"
        />
        <Icon
          class="icon"
          icon="simple-icons:zig"
          color="white"
          width="61"
          height="61"
        />
        <Icon
          class="icon"
          icon="teenyicons:c-solid"
          color="white"
          width="61"
          height="61"
        />
      </div>
    </div>
  </div>
</div>

<style>
  .wrapper {
    display: flex;
    flex-direction: column;
    align-items: center;
    padding: 8.125rem;
  }
  h1 {
    font-size: 2.5rem;
    font-weight: normal;
    text-align: center;
    margin-bottom: 7.5rem;
  }
  .button {
    display: flex;
    align-items: center;
    justify-content: center;
    border: 0.0625rem solid #9e9e9e;
    width: 44px;
    height: 44px;
    margin-bottom: 7.5rem;
    border-radius: 50%;
    animation: upDown 0.5s ease-in-out infinite alternate;
  }
  @keyframes upDown {
    0% {
      transform: translateY(-0.3125rem);
    }
    100% {
      transform: translateY(0.3125rem);
    }
  }
  h2 {
    font-size: 30px;
    font-weight: bold;
    text-align: center;
  }

  .skills {
    display: flex;
    justify-content: center;
    align-items: center;
    flex-wrap: wrap;
    gap: 4rem;
  }

  p {
    font-size: 1.5625rem;
    width: 100%;
    text-align: center;
    margin-bottom: 3.125rem;
  }
  .lower-sec {
    display: flex;
    flex-direction: column;
    gap: 6.25rem;
  }
  :global(.icon) {
    transition: 0.3s;
    transform: scale(1);
  }

  :global(.icon:hover) {
    transform: scale(1.2);
  }
</style>
