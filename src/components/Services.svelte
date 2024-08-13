<script>
  import ServiceCard from './ServiceCard.svelte';
  import SectionWrapper from './SectionWrapper.svelte';
  const services = [
    {
      title: 'Expand Your Business',
      highlightWord: 'Globally',
      intro:
        'Our international expansion services help you reach customers worldwide and navigate global markets effectively.',
      features: [
        'Market entry strategy development',
        'Cross-border e-commerce solutions',
        'International compliance assistance',
        'Localization and cultural adaptation',
      ],
      imgUrl: '/feature001.webp',
    },
    {
      title: 'Boost Your',
      highlightWord: 'Digital',
      titleSuffix: 'Marketing Impact',
      intro:
        'Enhance your online presence and reach with our comprehensive digital marketing strategies.',
      features: [
        'Social media campaign management',
        'SEO optimization techniques',
        'Content marketing strategies',
        'Analytics and performance tracking',
      ],
      imgUrl: '/feature002.webp',
    },
    {
      title: 'Comprehensive',
      highlightWord: 'Cybersecurity',
      titleSuffix: 'Solutions',
      intro:
        'Protect your digital assets with our multi-layered approach to cybersecurity.',
      features: [
        'Infrastructure security assessment',
        'Network vulnerability testing',
        'Project security reviews',
        'Cloud security implementation',
      ],
      imgUrl: '/feature003.webp',
    },
    {
      title: 'Business Process',
      highlightWord: 'Automation',
      intro:
        'Streamline your commercial processes with cutting-edge IT and AI technologies.',
      features: [
        'Workflow automation design',
        'AI-powered decision support systems',
        'Robotic Process Automation (RPA)',
        'Integration of IoT for data-driven operations',
      ],
      imgUrl: '/feature004.webp',
    },
  ];
</script>

<SectionWrapper id="services">
  <div
    class="mx-auto container flex flex-col gap-10 sm:gap-14 md:gap-24 flex-1 items-center justify-center"
  >
    <div class="flex flex-col gap-2">
      <p class="opacity-60 text-base sm:text-lg md:text-xl text-center">
        Start your digital <span class="text-teal-400 font-bold"
          >advancement</span
        > today
      </p>

      <h3
        class="text-4xl sm:text-5xl md:text-6xl max-w-[1000px] mx-auto w-full font-semibold text-center"
      >
        Innovative Solutions for Every Business
      </h3>
    </div>

    {#each services as service, index}
      <ServiceCard {service} {index} />
    {/each}
  </div>
</SectionWrapper>
