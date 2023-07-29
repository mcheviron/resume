<script>
  import knowledge from "$lib/assets/about.jpg";
  import Timeline from "$lib/components/Timeline.svelte";
  import typewriter from "$lib/typewriter";
</script>

<div class="flex p-12 lg:gap-60">
  <div class="lg:w-1/2">
    <div transition:typewriter={{ speed: 30 }}>
      <h1 class="md:text-4xl font-normal text-start">
        Hi, I'm Mostafa Elataby-Cheviron, I'm a software engineer and a
        fullstack developer. I love technology in all its forms and the general
        sciences. I don’t care if it’s OS internals or UI/UX design.
      </h1>
      <h2 class="md:text-4xl font-normal text-gray-400 mt-4 text-start">
        Knowledge shouldn’t have gate keepers.
      </h2>
    </div>
    <div class="mt-24 flex gap-7 items-center">
      <div
        class="flex items-center justify-center border-[0.065rem] border-solid border-[#9e9e9e] w-11 h-11 rounded-full animate-bounce"
      >
        <svg
          class="w-4 h-4 md:w-6 md:h-6"
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
      <p class="md:text-2xl">Know more about me</p>
    </div>
  </div>
  <div class="hidden lg:block">
    <img
      src={knowledge}
      alt="knwoledge"
      class="object-cover h-[37.5rem] rounded-md transition duration-300 hover:scale-105"
    />
  </div>
</div>
<div class="flex justify-center items-center">
  <Timeline />
</div>
<h2
  class="flex items-center justify-center text-lg md:text-4xl font-normal mt-16 mb-10 md:mb-0"
>
  Code
</h2>
<div class="hidden md:flex flex-col gap-3 my-48 mx-9 lg:mx-0">
  <p class="text-4xl font-normal w-[47rem]">
    Other interests that have nothing to do with business:
  </p>
  <ul class="m-10">
    <li>I was a swimming champion and played it for over 15 years</li>
    <li>I was a fencer as well but played it much less than swimming</li>
    <li>I am an avid reader, especially non-fiction, history and philosophy</li>
    <li>I have a cat and she’s our daughter</li>
    <li>
      I speak four languages fluently and others with a lower degree of fluency
    </li>
  </ul>
</div>

<style>
  li {
    margin: 20px 0;
    font-size: 1.875rem;
    font-weight: normal;
  }
  ul {
    margin: 0 1.25rem;
    list-style-type: circle;
  }
</style>
