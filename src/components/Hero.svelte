<script>
  import Header from './Header.svelte';
  import SectionWrapper from './SectionWrapper.svelte';
  import Partners from './Partners.svelte';
</script>

<div class="bg-gradient-to-r from-teal-50 to-purple-50 w-full">
  <Header />
  <SectionWrapper>
    <div
      class="mx-auto container flex flex-col gap-10 flex-1 items-center justify-center"
    >
      <h2
        class="text-5xl sm:text-6xl md:text-7xl lg:text-8xl mx-auto w-full text-center font-semibold"
      >
        <span class="text-black align-text-bottom">Empowering </span>
        <span class="text-teal-400 italic poppins align-text-bottom"
          >Innovations</span
        ><br />
        <span class="text-black align-text-bottom"
          >for a Technological Future</span
        >
      </h2>
      <p
        class="text-xl sm:text-2xl md:text-3xl text-center max-w-[1000px] mx-auto w-full"
      >
        Less complexity, more efficiency. We're the IT experts by your side,
        providing tailored solutions, technological insights, performance
        analytics, and much more for your business success.
      </p>
      <div class="flex items-center gap-4">
        <a
          href="#contact"
          class="py-2 px-4 rounded-lg bg-teal-500 text-white hover:bg-teal-400 disabled:opacity-50 disabled:pointer-events-none"
        >
          <p
            class="w-full sm:w-auto inline-flex justify-center items-center gap-x-2 text-base md:text-lg font-normal"
          >
            Contact Us
          </p>
        </a>
        <a
          href="#services"
          class="border border-black bg-white py-2 px-4 rounded-lg"
        >
          <p class="text-base sm:text-lg md:text-xl">Explore Services &rarr;</p>
        </a>
      </div>
      <div class="flex justify-center space-x-12 mt-6 mb-4">
        <div class="transition transform hover:scale-110">
          <h3 class="text-2xl text-center font-bold">500+</h3>
          <p class="text-zinc-400 font-semibold">Successful cases</p>
        </div>
        <div class="transition transform hover:scale-110">
          <h3 class="text-2xl text-center font-bold">20+</h3>
          <p class="text-zinc-400 font-semibold">Years of Experience</p>
        </div>
      </div>
    </div>
    <Partners />
  </SectionWrapper>
</div>
