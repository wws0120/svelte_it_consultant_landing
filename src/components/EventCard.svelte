<script>
  export let eventContent;
</script>

<div class="relative rounded-t-xl shadow shadow-gray-700 overflow-hidden">
  <img class="aspect-[4/3] object-cover" src={eventContent.image} alt="" />

  <div class=" p-6">
    <a
      href="/"
      class="text-lg hover:text-teal-500 transition duration-500 ease-in-out font-medium h5"
      >{eventContent.title}</a
    >
    <p class="text-slate-400 mt-3">
      {eventContent.description}
    </p>

    <div class="mt-5">
      <a
        href={eventContent.link}
        class="hover:text-teal-500 after:bg-teal-600 transition duration-500"
        >Read More <i class="uil uil-arrow-right" /></a
      >
    </div>
  </div>
</div>
