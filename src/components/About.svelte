<script>
  import SectionWrapper from './SectionWrapper.svelte';
  import {
    IconTransformPoint,
    IconRobot,
    IconCloudDataConnection,
    IconPresentationAnalytics,
    IconCloudLock,
    IconBrowserCheck,
  } from '@tabler/icons-svelte';
</script>

<section id="about" class="relative overflow-hidden">
  <SectionWrapper>
    <div class="container mx-auto">
      <div
        class="grid lg:grid-cols-12 grid-cols-1 items-center gap-y-16 lg:gap-8"
      >
        <div class="lg:col-span-7">
          <div class="md:me-2">
            <span
              class="inline-flex items-center rounded-full text-2xl font-semibold mb-6"
            >
              Transform Your Business
            </span>
            <h4 class="text-3xl font-bold capitalize mb-4">
              <span
                class="bg-gradient-to-l from-teal-300 to-teal-500 text-transparent bg-clip-text"
                >Innovate & Optimize</span
              > With Expert IT Solutions
            </h4>
            <p class="text-lg max-w-xl text-default-200 mb-6">
              We are a leading IT consultancy dedicated to connecting businesses
              with cutting-edge technology solutions and expert strategies for
              digital transformation!
            </p>
            <div>
              <div class="grid md:grid-cols-2 gap-4 py-6 text-lg font-semibold">
                <div class="flex gap-3 items-center">
                  <IconTransformPoint class="text-orange-500" />
                  <p>Digital transformation</p>
                </div>

                <div class="flex gap-3 items-center">
                  <IconCloudDataConnection class="text-orange-500" />
                  <p>Cloud solutions</p>
                </div>

                <div class="flex gap-3 items-center">
                  <IconCloudLock class="text-orange-500" />
                  <p>Cybersecurity measures</p>
                </div>

                <div class="flex gap-3 items-center">
                  <IconBrowserCheck class="text-orange-500" />
                  <p>Social marketing strategy</p>
                </div>
                <div class="flex gap-3 items-center">
                  <IconRobot class="text-orange-500" />
                  <p>AI integration</p>
                </div>
                <div class="flex gap-3 items-center">
                  <IconPresentationAnalytics class="text-orange-500" />
                  <p>Data analytics</p>
                </div>
              </div>
            </div>
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
          <div class="flex gap-4 md:gap-6 tilt">
            <div class="flex flex-col gap-4 md:gap-6 pt-10 md:pt-16 w-full">
              <img
                src="/pic00d.webp"
                class="w-full h-40 md:h-[278px] rounded-lg object-cover"
                alt=""
              />
              <img
                src="/pic00c.webp"
                class="w-full h-40 md:h-[278px] rounded-lg object-cover"
                alt=""
              />
            </div>
            <div
              class="flex flex-col gap-4 md:gap-6 pb-10 md:pb-16 w-full relative"
            >
              <div class="absolute bottom-0 end-0 -z-10">
                <i
                  data-lucide="triangle"
                  class="animate-[spin_10s_linear_infinite] h-12 w-12 fill-primary/20 text-transparent"
                ></i>
              </div>
              <img
                src="/pic00b.webp"
                class="w-full h-40 md:h-[278px] rounded-lg object-cover"
                alt=""
              />
              <img
                src="/pic00a.webp"
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
