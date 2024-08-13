<script>
  import {
    IconBrandInstagram,
    IconBrandDiscord,
    IconBrandFacebook,
    IconBrandTwitter,
  } from '@tabler/icons-svelte';

  const menuList = [
    { name: 'Home', url: '/' },
    { name: 'About', url: '#about' },
    { name: 'Services', url: '#services' },
    { name: 'Reviews', url: '#reviews' },
    { name: 'FAQs', url: '#faqs' },
    { name: 'Events', url: '#events' },
    { name: 'Contact', url: '#contact' },
  ];
</script>

<footer class="py-16 sm:py-20 md:py-24 px-4 md:px-8">
  <div
    class="container mx-auto w-full grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-6 gap-8 text-base"
  >
    <div class="flex flex-col gap-4 md:col-span-3">
      <h1 class="font-semibold">
        Nex<span class="text-teal-400">Gen</span> Solutions
      </h1>
      <p>©2024 NEXGEN SOLUTIONS LTD. All rights reserved.</p>
    </div>
    <div class="flex flex-col gap-4 md:col-span-2">
      <p class="font-bold text-lg md:text-xl">Useful link</p>

      <div class="grid grid-cols-2 gap-x-4 gap-y-2 max-w-xs">
        {#each menuList as item}
          <a
            href={item.url}
            class="cursor-pointer pr-2 hover:text-teal-400 duration-200"
          >
            {item.name}
          </a>
        {/each}
      </div>
    </div>
    <div class="flex flex-col gap-4">
      <p class="font-bold text-base sm:text-lg">Follow Us</p>
      <a
        href="/"
        target="_blank"
        class="cursor-pointer hover:text-teal-400 duration-200"
      >
        <IconBrandInstagram size={28} class="inline-block pr-2" />
        Instagram</a
      >
      <a
        href="/"
        target="_blank"
        class="cursor-pointer hover:text-teal-400 duration-200"
      >
        <IconBrandFacebook size={28} class="inline-block pr-2" />
        Facebook</a
      >
      <a
        href="/"
        target="_blank"
        class="cursor-pointer hover:text-teal-400 duration-200"
      >
        <IconBrandTwitter size={28} class="inline-block pr-2" />
        Twitter</a
      >
      <a
        href="/"
        target="_blank"
        class="cursor-pointer hover:text-teal-400 duration-200"
      >
        <IconBrandDiscord size={28} class="inline-block pr-2" />
        Discord</a
      >
    </div>
  </div>
</footer>
