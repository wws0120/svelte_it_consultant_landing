<script>
  import SectionWrapper from './SectionWrapper.svelte';

  import {
    IconRocket,
    IconBriefcase,
    IconCertificate,
  } from '@tabler/icons-svelte';
</script>

<section>
  <SectionWrapper>
    <div class="container mx-auto">
      <div class="grid grid-cols-12 gap-y-16 lg:gap-8 items-center">
        <div class="col-span-12 lg:col-span-7 lg:order-2">
          <div class="mb-6">
            <div class="text-2xl font-semibold text-teal-400 mb-4">
              Why Choose Us?
            </div>
            <h2 class="text-3xl font-bold mb-6">
              Strategic Innovation Meets IT Excellence
            </h2>
            <p class="text-lg text-gray-600">
              We are a team committed to leveraging sophisticated IT strategies
              to elevate businesses. Our approach integrates cutting-edge
              technology with creative problem-solving to enhance productivity,
              expand market share, and optimize costs, thereby delivering
              tangible results and a competitive edge.
            </p>
            <ul class=" space-y-2 pt-8">
              <li class="flex flex-wrap">
                <div class="flex-none mr-3">
                  <IconRocket class="text-orange-500" />
                </div>
                <div class="flex-1">
                  <h4 class=" text-lg mb-1 font-semibold">
                    95% Client Success Rate
                  </h4>
                </div>
              </li>
              <li class="flex flex-wrap">
                <div class="flex-none mr-3">
                  <IconBriefcase class="text-orange-500" />
                </div>
                <div class="flex-1">
                  <h4 class=" text-lg mb-1 font-semibold">
                    500+ Projects Delivered
                  </h4>
                </div>
              </li>
              <li class="flex flex-wrap">
                <div class="flex-none mr-3">
                  <IconCertificate class="text-orange-500" />
                </div>
                <div class="flex-1">
                  <h4 class=" text-lg mb-1 font-semibold">
                    Industry-Leading Expertise
                  </h4>
                </div>
              </li>
            </ul>
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
        <div class="col-span-12 lg:col-span-5 lg:order-1">
          <div class="grid grid-cols-12 gap-6">
            <div class="col-span-6">
              <img class="rounded-lg" src="/pic001.webp" alt="" />
            </div>
            <div class="col-span-6">
              <img class="rounded-lg" src="/pic004.webp" alt="" />
            </div>
            <div class="col-span-12 px-4">
              <img class="rounded-lg" src="/pic002.webp" alt="" />
            </div>
          </div>
        </div>
      </div>
    </div>
  </SectionWrapper>
</section>
