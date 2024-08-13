<script>
  import SectionWrapper from './SectionWrapper.svelte';
  import TeamMember from './TeamMember.svelte';

  const team = [
    {
      title: 'Chief Technology Officer',
      name: 'Emily Zhang',
      imgUrl: '/p003.webp',
    },
    {
      title: 'Head of Digital Marketing',
      name: 'Sarah Johnson',
      imgUrl: '/p002.webp',
    },
    {
      title: 'VP of Global Strategy',
      name: 'Alexander Müller',
      imgUrl: '/p001.webp',
    },
  ];
</script>

<div id="team">
  <SectionWrapper>
    <div class="mx-auto container">
      <div class="grid grid-cols-1 pb-8 lg:pb-10 text-center">
        <p class="opacity-60 text-base sm:text-lg md:text-xl text-center">
          Meet the Minds Behind Our Success
        </p>
        <h3
          class="text-4xl sm:text-5xl md:text-6xl max-w-[1000px] mx-auto w-full font-semibold text-center"
        >
          Experts Committed to Your <span class="text-teal-400 font-bold"
            >Transformation
          </span>
        </h3>
      </div>
      <div class="grid lg:grid-cols-3 md:grid-cols-2 grid-cols-1 pt-8 gap-8">
        {#each team as member}
          <TeamMember {member} />
        {/each}
      </div>
    </div>
  </SectionWrapper>
</div>
