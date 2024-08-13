<script>
  export let review;
</script>

<div class="rounded-lg shadow-lg p-6 bg-white">
  <div class="flex items-center pb-6 border-b border-gray-100">
    <img src={review.image} class="h-16 w-16 rounded-full shadow" alt="" />

    <div class="pl-4">
      <p class="text-lg font-semibold">
        {review.name}
      </p>
      <p class="text-slate-400">{review.title}</p>
    </div>
  </div>

  <div class="mt-6">
    <p class="text-slate-500">
      {review.review}
    </p>
  </div>
</div>
