<script>
  export let index;
  export let service;
  import { IconRosetteDiscountCheck } from '@tabler/icons-svelte';
</script>

<div
  class="grid grid-cols-1 lg:grid-cols-2 gap-14 md:gap-14 lg:gap-20 relative text-base"
>
  <div
    class={'flex flex-col gap-8 md:gap-10 pt-8 sm:pt-10 ' +
      (index % 2 === 1 ? ' lg:order-2' : ' ')}
  >
    <h4
      class="text-2xl sm:text-3xl md:text-4xl max-w-[1000px] w-full font-medium relative pr-10 after:absolute after:top-full after:left-0 after:w-1/6 after:h-1 after:mt-1 after:bg-slate-500"
    >
      {service.title}
      <span class="text-teal-400">{service.highlightWord}</span>
      {service.titleSuffix || ''}
    </h4>
    <p>{service.intro}</p>
    <div class="flex flex-col gap-3">
      {#each service.features as listItem}
        <div class="flex gap-2 items-center">
          <IconRosetteDiscountCheck class="text-orange-400" size={24} />

          <p>{listItem}</p>
        </div>
      {/each}
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
  <div class={'flex flex-col shawdow overflow-hidden rounded-lg '}>
    <div class="flex flex-col bg-white gap-4 flex-1">
      <img
        src={service.imgUrl}
        class="object-cover w-full h-full"
        alt="service-img"
      />
    </div>
  </div>
</div>
