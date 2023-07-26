<script>
  import home from "$lib/assets/home.jpg";
</script>

<div
  class="flex flex-col justify-center items-center md:flex-row md:items-start md:justify-center md:gap-80 md:p-14"
>
  <div class="flex flex-col md:w-2/5 md:gap-40">
    <h1 class="text-4xl font-normal mb-32 w-80">
      Technophile, engineer, developer.
    </h1>
    <div class="flex flex-col space-y-6">
      <a href="/about" class="no-underline text-inherit w-44 h-16">
        <div
          class="hover:text-gray-600 inline-flex items-center justify-center bg-white text-black py-7 px-12 text-lg cursor-pointer rounded-full w-44 h-16"
        >
          About me
        </div>
      </a>
      <a href="/skills" class="no-underline text-inherit w-44 h-16">
        <div
          class="inline-flex items-center justify-center bg-[#1f2028] text-white py-7 px-12 text-lg cursor-pointer rounded-full border-2 border-solid border-gray-600 w-44 h-16 transition duration-300 hover:border-2 hover:border-solid hover:border-[#1f2028]"
        >
          Skills
        </div>
      </a>
      <a href="/projects" class="no-underline text-inherit w-44 h-16 md:hidden">
        <div
          class="inline-flex items-center justify-center bg-[#1f2028] text-white py-7 px-12 text-lg cursor-pointer rounded-full border-2 border-solid border-gray-600 w-44 h-16 transition duration-300 hover:border-2 hover:border-solid hover:border-[#1f2028]"
        >
          Projects
        </div>
      </a>
    </div>
  </div>
  <div class="">
    <img
      src={home}
      alt="monitors with code"
      class="hidden object-cover h-[37.5rem] w-full rounded-md transition ease-out duration-300 hover:scale-105 lg:block"
    />
  </div>
</div>
