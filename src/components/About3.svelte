<script>
  import SectionWrapper from './SectionWrapper.svelte';
  import {
    IconHeartHandshake,
    IconZoomCheck,
    IconTool,
    IconChartLine,
  } from '@tabler/icons-svelte';
</script>

<section id="about" class="relative overflow-hidden">
  <SectionWrapper>
    <div class="container mx-auto">
      <div
        class="grid lg:grid-cols-12 grid-cols-1 items-center gap-y-16 lg:gap-8"
      >
        <div class="lg:col-span-7">
          <div>
            <span
              class="inline-flex items-center rounded-full text-2xl font-semibold mb-6"
              >Our Approach</span
            >
            <h4 class="text-3xl font-bold capitalize mb-4">
              Collaborative <span
                class="bg-gradient-to-l from-teal-300 to-teal-500 text-transparent bg-clip-text"
                >Excellence</span
              > in Action
            </h4>
            <p class="text-lg text-default-200 mb-6">
              At NexGen Solutions, we believe in the power of collaboration and
              tailored solutions. Our team of seasoned experts works closely
              with you to understand your unique challenges and goals, crafting
              bespoke strategies that drive real-world results.
            </p>
            <ul class="flex flex-wrap gap-5 py-6 max-w-2xl">
              <li
                class="flex space-x-2.5 items-center text-teal-500 font-semibold px-5 py-3 bg-gray-50 border border-purple-100 leading-none rounded-full"
              >
                ,

                <span>
                  <IconHeartHandshake class="text-orange-400" />
                </span>
                <span>Client-Centric Partnership</span>
              </li>
              <li
                class="flex space-x-2.5 items-center text-teal-500 font-semibold px-5 py-3 bg-gray-50 border border-purple-100 leading-none rounded-full"
              >
                <span>
                  <IconZoomCheck class="text-orange-400" />
                </span>
                <span>In-Depth Analysis & Planning</span>
              </li>
              <li
                class="flex space-x-2.5 items-center text-teal-500 font-semibold px-5 py-3 bg-gray-50 border border-purple-100 leading-none rounded-full"
              >
                <span>
                  <IconTool class="text-orange-400" />
                </span>
                <span>Agile Implementation</span>
              </li>
              <li
                class="flex space-x-2.5 items-center text-teal-500 font-semibold px-5 py-3 bg-gray-50 border border-purple-100 leading-none rounded-full"
              >
                <span>
                  <IconChartLine class="text-orange-400" />
                </span>
                <span>Continuous Improvement</span>
              </li>
            </ul>
            <div class="flex items-center">
              <a
                class="w-full sm:w-auto py-2 px-4 inline-flex justify-center items-center gap-x-2 text-base md:text-lg font-normal rounded-lg bg-teal-500 text-white hover:bg-teal-400 disabled:opacity-50 disabled:pointer-events-none"
                href="#contact"
              >
                Contact Us
              </a>
            </div>
          </div>
        </div>

        <div class="lg:col-span-5">
          <div class="flex gap-4 md:gap-6 items-center">
            <div class="flex flex-col gap-4 md:gap-6 w-full">
              <img
                src="/about03a.webp"
                class="h-full w-full rounded-lg object-cover"
                alt=""
              />
            </div>
            <div
              class="flex flex-col gap-4 md:gap-6 pb-10 md:pb-16 w-full relative"
            >
              <img
                src="/about03b.webp"
                class="w-full h-40 md:h-[278px] rounded-lg object-cover"
                alt=""
              />
              <img
                src="/about03c.webp"
                class="w-full h-40 md:h-[278px] rounded-lg object-cover"
                alt=""
              />
            </div>
          </div>
        </div>
      </div>
    </div>
  </SectionWrapper>
</section>
