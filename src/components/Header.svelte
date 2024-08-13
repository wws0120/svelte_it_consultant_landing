<script>
  import { IconX, IconMenu2 } from '@tabler/icons-svelte';
  let isMenuOpen = false;
  const mobileMenuList = [
    { name: 'Home', url: '/' },
    { name: 'About', url: '#about' },
    { name: 'Services', url: '#services' },
    { name: 'Reviews', url: '#reviews' },
    { name: 'FAQs', url: '#faqs' },
    { name: 'Events', url: '#events' },
    { name: 'Contact', url: '#contact' },
  ];

  const menuList = mobileMenuList.filter((item) => item.name !== 'Home');

  function toggleMenu() {
    isMenuOpen = !isMenuOpen;
  }
</script>

<header
  class="flex flex-col relative bg-gradient-to-r from-teal-50 to-purple-50 z-20"
>
  <div
    class="  max-w-[1400px] mx-auto w-full flex items-center justify-between p-4 py-6"
  >
    <a href="/">
      <h1 class="text-2xl font-semibold">
        Nex<span class="text-teal-400">Gen</span> Solutions
      </h1>
    </a>

    <nav class="hidden md:flex items-center gap-4 lg:gap-6">
      {#each menuList as item}
        <a
          href={item.url}
          class="duration-200 hover:text-teal-400 text-xl font-normal cursor-pointer"
          >{item.name}</a
        >
      {/each}
    </nav>
    <button class="md:hidden" on:click={toggleMenu}>
      {#if isMenuOpen}
        <IconX size={28} />
      {:else}
        <IconMenu2 size={28} />
      {/if}
    </button>
  </div>
  {#if isMenuOpen}
    <nav
      class="md:hidden absolute top-full left-0 right-0 bg-slate-50 shadow-lg"
    >
      {#each mobileMenuList as item}
        <a
          href={item.url}
          class="block py-4 px-4 text-2xl font-normal text-center hover:bg-gray-100 hover:text-teal-400"
          on:click={toggleMenu}
        >
          {item.name}
        </a>
      {/each}
    </nav>
  {/if}
</header>
