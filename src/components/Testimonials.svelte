<script>
  import TestimonialCard from './TestimonialCard.svelte';
  import SectionWrapper from './SectionWrapper.svelte';

  const clientReviews = [
    {
      image: '/avatar001.webp',
      name: 'Alex Novak',
      title: 'CEO, Global Tech Solutions',
      review:
        "Working with this IT consultancy has been a game-changer for our company. Their expertise in automation and data analysis has significantly improved our operational efficiency. We've seen a 30% increase in productivity within just six months!",
    },
    {
      image: '/avatar003.webp',
      name: 'Daniel Kim',
      title: 'CTO, InnovateNow Corp',
      review:
        "The cybersecurity solutions provided by this team are top-notch. They identified vulnerabilities we weren't even aware of and implemented robust security measures. I can now sleep soundly knowing our data is well-protected.",
    },
    {
      image: '/avatar002.webp',
      name: 'Sophia Lee',
      title: 'Marketing Director, E-commerce Pioneer',
      review:
        "Their digital marketing strategies have revolutionized our online presence. We've seen a 150% increase in organic traffic and a 200% boost in lead generation. The ROI on their services has been phenomenal!",
    },
    {
      image: '/avatar004.webp',
      name: 'Emma Thompson',
      title: 'COO, Fintech Innovators',
      review:
        'The project management and optimization services we received were outstanding. They streamlined our processes, reducing project delivery times by 40%. Their insights have been invaluable to our growth.',
    },
    {
      image: '/avatar005.webp',
      name: 'Neil Patel',
      title: 'Head of Data Science, HealthTech Solutions',
      review:
        'The data analysis capabilities of this team are extraordinary. They helped us make sense of our complex healthcare data, leading to improved patient outcomes and a 25% reduction in operational costs.',
    },
    {
      image: '/avatar006.webp',
      name: 'John Martinez',
      title: 'Founder, AI Startups Inc',
      review:
        'As a startup in the AI space, we needed guidance on both technical and strategic fronts. This consultancy provided exactly that. Their insights helped us secure funding and accelerate our product development by months.',
    },
  ];
</script>

<section class="relative bg-gray-50" id="reviews">
  <SectionWrapper>
    <div class="container mx-auto">
      <div class="grid grid-cols-1 pb-8 md:pb-10 text-center">
        <p class="opacity-60 text-base sm:text-lg md:text-xl text-center">
          Real Stories from Satisfied Clients
        </p>
        <h3
          class="text-4xl sm:text-5xl md:text-6xl max-w-[1000px] mx-auto w-full font-semibold text-center"
        >
          Discover Why Businesses <span class="text-teal-400 font-bold"
            >Trust</span
          > Our Expertise
        </h3>
      </div>

      <div
        class="grid lg:grid-cols-3 sm:grid-cols-2 grid-cols-1 mt-8 gap-[30px]"
      >
        {#each clientReviews as review}
          <TestimonialCard {review} />
        {/each}
      </div>
    </div>
  </SectionWrapper>
</section>
