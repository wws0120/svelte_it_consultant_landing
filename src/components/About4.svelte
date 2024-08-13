<script>
  import SectionWrapper from './SectionWrapper.svelte';
  import {
    IconTelescope,
    IconGolf,
    IconShieldLock,
  } from '@tabler/icons-svelte';
</script>

<section>
  <SectionWrapper>
    <div class="container mx-auto">
      <div class="flex flex-col gap-2 pb-8 lg:pb-10">
        <p class="opacity-60 text-base sm:text-lg md:text-xl text-center">
          Our Core Principles
        </p>
        <h3
          class="text-4xl sm:text-5xl md:text-6xl max-w-[1000px] mx-auto w-full font-semibold text-center"
        >
          <span class="text-teal-400 font-bold">Guiding Vision</span> and
          <span class="text-teal-400 font-bold">Mission</span>
        </h3>
      </div>
      <div class="md:flex md:items-center gap-7 pt-8">
        <div
          class="flex flex-1 flex-col items-start gap-5 transition-all duration-300 hover:translate-y-[-3px] mb-12 md:mb-0"
        >
          <div class="bg-teal-100 p-3 rounded-full">
            <IconTelescope size={32} class="text-slate-800" />
          </div>
          <div>
            <h3 class="font-extrabold text-2xl mb-2">Our Vision</h3>
            <p class="text-excerpt">
              To be the most trusted and innovative IT consulting partner,
              shaping the digital landscape of businesses worldwide, globally,
              and comprehensively.
            </p>
          </div>
        </div>
        <div
          class="flex flex-1 flex-col items-start gap-5 transition-all duration-300 hover:translate-y-[-3px] mb-12 md:mb-0"
        >
          <div class="bg-teal-100 p-3 rounded-full">
            <IconGolf size={32} class="text-slate-800" />
          </div>
          <div>
            <h3 class="font-extrabold text-2xl mb-2">Our Mission</h3>
            <p class="text-excerpt">
              To deliver transformative IT solutions that drive business growth,
              enhance operational efficiency, and secure digital futures for our
              clients.
            </p>
          </div>
        </div>
        <div
          class="flex flex-1 flex-col items-start gap-5 transition-all duration-300 hover:translate-y-[-3px] mb-12 md:mb-0"
        >
          <div class="bg-teal-100 p-3 rounded-full">
            <IconShieldLock size={32} class="text-slate-800" />
          </div>
          <div>
            <h3 class="font-extrabold text-2xl mb-2">Our Values</h3>
            <p class="text-excerpt">
              To embody excellence, integrity, and innovation, while
              prioritizing client-centric solutions and continuous learning for
              lasting impact.
            </p>
          </div>
        </div>
      </div>
    </div>
  </SectionWrapper>
</section>
