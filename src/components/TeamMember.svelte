<script>
  import {
    IconBrandInstagram,
    IconBrandTwitter,
    IconBrandMeta,
  } from '@tabler/icons-svelte';
  export let member;
</script>

<div class="relative rounded-xl overflow-hidden group">
  <div class="w-full">
    <img class="w-full h-[480px] object-cover" src={member.imgUrl} alt="" />
  </div>

  <div class="absolute bottom-0 inset-x-0 m-2">
    <div class="p-4 bg-white rounded-lg">
      <div class="mt-1">
        <h2 class="text-2xl font-bold flex items-center">{member.name}</h2>
      </div>
      <h2 class="text-lg text-neutral-500 font-medium mb-1">
        {member.title}
      </h2>
    </div>
  </div>

  <div
    class="absolute inset-0 h-full flex items-center justify-center opacity-0 group-hover:opacity-100 transition-all duration-500"
  >
    <ul class="mb-4 space-x-2 justify-start p-4">
      <li class="inline-block">
        <a
          href="/"
          class="h-10 w-10 inline-flex items-center justify-center tracking-wide align-middle duration-500 text-base text-center rounded-lg bg-white"
          ><IconBrandInstagram class=" text-gray-500" size={28} stroke={2} /></a
        >
      </li>
      <li class="inline-block">
        <a
          href="/"
          class="h-10 w-10 inline-flex items-center justify-center tracking-wide align-middle duration-500 text-base text-center rounded-lg bg-white"
          ><IconBrandTwitter class=" text-gray-500" size={28} stroke={2} /></a
        >
      </li>
      <li class="inline-block">
        <a
          href="/"
          class="h-10 w-10 inline-flex items-center justify-center tracking-wide align-middle duration-500 text-base text-center rounded-lg bg-white"
          ><IconBrandMeta class=" text-gray-500" size={28} stroke={2} /></a
        >
      </li>
    </ul>
    <!--end social -->
  </div>
</div>
