<script>
  import SectionWrapper from './SectionWrapper.svelte';
  import {
    IconZoom,
    IconChartInfographic,
    IconBrowserCheck,
    IconTransform,
  } from '@tabler/icons-svelte';

  const steps = [
    {
      icon: IconZoom,
      title: 'Discovery and Analysis',
      description: [
        'Understand your business needs and challenges',
        'Analyze current systems and processes',
        'Identify opportunities for improvement',
      ],
    },
    {
      icon: IconChartInfographic,
      title: 'Strategic Planning',
      description: [
        'Develop a tailored technology roadmap',
        'Set measurable goals and KPIs',
        'Create a detailed project timeline',
      ],
    },
    {
      icon: IconBrowserCheck,
      title: 'Implementation and Integration',
      description: [
        'Execute the planned solutions',
        'Seamlessly integrate new technologies',
        'Provide training and support for your team',
      ],
    },
    {
      icon: IconTransform,
      title: 'Continuous Optimization',
      description: [
        'Monitor performance and gather feedback',
        'Make data-driven adjustments',
        'Ensure long-term success and scalability',
      ],
    },
  ];
</script>

<section class="bg-teal-50">
  <SectionWrapper>
    <div class="container mx-auto">
      <div class="flex flex-col gap-2 pb-8 md:pb-10">
        <h2 class="opacity-60 text-base sm:text-lg md:text-xl text-center">
          Our Working Process
        </h2>
        <p
          class="text-4xl sm:text-5xl md:text-6xl max-w-[1000px] mx-auto w-full font-semibold text-center leading-relax sm:leading-relax md:leading-relax"
        >
          <span class="text-teal-400">Step-by-Step</span> Guide to Achieving Your
          Business Goals TEST
        </p>
      </div>
      <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 pt-8 gap-8">
        {#each steps as step}
          <div class="bg-white p-6 rounded-lg shadow-md">
            <div
              class="flex items-center justify-center w-14 h-14 bg-teal-400 text-white rounded-full mb-4"
            >
              <svelte:component this={step.icon} size={30} />
            </div>
            <h3 class="text-xl font-semibold mb-4">{step.title}</h3>
            <ul class="list-disc list-inside text-gray-600">
              {#each step.description as item}
                <li>{item}</li>
              {/each}
            </ul>
          </div>
        {/each}
      </div>
    </div>
  </SectionWrapper>
</section>
