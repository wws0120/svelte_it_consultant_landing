<script>
  import SectionWrapper from './SectionWrapper.svelte';
  import EventCard from './EventCard.svelte';
  const events = [
    {
      image: '/event001.webp',
      title: 'AI in Business Workshop',
      description:
        'Learn how to leverage artificial intelligence to streamline operations and boost productivity in this hands-on, interactive workshop.',
      link: '/',
      color: 'teal',
    },
    {
      image: '/event002.webp',
      title: 'Future Tech Summit 2024',
      description:
        'Explore cutting-edge innovations and their impact on business efficiency in this two-day conference featuring industry leaders and tech visionaries.',
      link: '/',
      color: 'teal',
    },
    {
      image: '/event003.webp',
      title: 'Cybersecurity Symposium',
      description:
        'Join cybersecurity experts to discuss the latest threats and strategies for protecting your business in an increasingly digital world.',
      link: '/',
      color: 'teal',
    },
  ];
</script>

<section class="relative" id="events">
  <SectionWrapper>
    <div class="container mx-auto">
      <div class="grid grid-cols-1 pb-8 lg:pb-10 text-center">
        <p class="opacity-60 text-base sm:text-lg md:text-xl text-center">
          Highlights from Our Knowledge-Sharing Events
        </p>

        <h3
          class="text-4xl sm:text-5xl md:text-6xl max-w-[1000px] mx-auto w-full font-semibold text-center"
        >
          Our Featured Events
        </h3>
      </div>

      <div
        class="grid grid-cols-1 lg:grid-cols-3 md:grid-cols-2 gap-[30px] mt-8"
      >
        {#each events as eventContent}
          <EventCard {eventContent} />
        {/each}
      </div>
    </div>
  </SectionWrapper>
</section>
