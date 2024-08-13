<script>
  import SectionWrapper from './SectionWrapper.svelte';

  let faqs = [
    {
      question: 'What services does your IT consultancy offer?',
      answer:
        'We offer a wide range of services including digital transformation strategy, cybersecurity solutions, cloud migration, data analytics, custom software development, and IT infrastructure optimization.',
    },
    {
      question: 'How can your services benefit my business?',
      answer:
        'Our services can help streamline your operations, enhance security, improve decision-making through data insights, reduce IT costs, and give you a competitive edge in the digital landscape.',
    },
    {
      question: 'Do you work with businesses of all sizes?',
      answer:
        'Yes, we cater to businesses of all sizes, from startups to large enterprises. We tailor our solutions to meet the specific needs and scale of each client.',
    },
    {
      question: "What's your approach to ensuring client confidentiality?",
      answer:
        'We take client confidentiality very seriously. We implement strict data protection measures, use secure communication channels, and adhere to all relevant privacy laws and regulations.',
    },
    {
      question: 'How long does a typical IT consultancy project take?',
      answer:
        'Project duration varies depending on the scope and complexity. Some projects may take a few weeks, while others could span several months. We provide detailed timelines during our initial consultation.',
    },
    {
      question: 'What makes your IT consultancy different from others?',
      answer:
        'We combine cutting-edge technical expertise with a deep understanding of business strategy. Our solutions are not just technically sound but also aligned with your business goals for maximum impact.',
    },
  ];

  let activeIndex = -1;

  function toggleAnswer(index) {
    activeIndex = activeIndex === index ? -1 : index;
  }
</script>

<div id="faqs" class="flex flex-col flex-1 items-center justify-center">
  <SectionWrapper>
    <div class="container flex flex-col gap-2 pb-8 lg:pb-10">
      <p class="opacity-60 text-base sm:text-lg md:text-xl text-center">
        Answers to Your Top IT Consultancy Queries
      </p>
      <h3
        class="text-4xl sm:text-5xl md:text-6xl max-w-[1000px] mx-auto w-full font-semibold text-center"
      >
        Frequently Asked Questions
      </h3>
    </div>

    <div class="max-w-3xl w-full mx-auto pt-8">
      {#each faqs as faq, index}
        <div class="mb-4 border-b border-gray-200 pb-4">
          <button
            class="flex justify-between items-center w-full text-left"
            on:click={() => toggleAnswer(index)}
          >
            <span class="text-base sm:text-lg md:text-xl font-semibold"
              >{faq.question}</span
            >
            <span class="text-teal-400 text-2xl"
              >{activeIndex === index ? '−' : '+'}</span
            >
          </button>
          {#if activeIndex === index}
            <p class="mt-3 text-base sm:text-lg md:text-xl text-gray-600">
              {faq.answer}
            </p>
          {/if}
        </div>
      {/each}
    </div>
  </SectionWrapper>
</div>
