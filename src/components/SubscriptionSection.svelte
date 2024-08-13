<script>
  let email = '';

  function handleSubmit() {
    console.log('Subscribed with email:', email);
    email = '';
  }
</script>

<div class="bg-gradient-to-r from-blue-500 to-green-500 text-white">
  <div class="container mx-auto px-6 py-24 text-center">
    <h1 class="text-4xl md:text-6xl font-bold mb-4">
      Stay Updated with Our Latest IT Solutions
    </h1>
    <p class="font-mono text-xl md:text-2xl mb-8">
      Subscribe to receive updates on automation, digital marketing, security,
      and data analysis
    </p>
    <form
      on:submit|preventDefault={handleSubmit}
      class="flex flex-col md:flex-row justify-center items-center"
    >
      <input
        type="email"
        placeholder="Enter your email"
        bind:value={email}
        class="bg-white text-teal-500 font-bold py-2 px-4 rounded-xl mb-4 md:mb-0 md:mr-4 w-full md:w-auto"
        required
      />
      <button
        type="submit"
        class="bg-white text-teal-400 font-bold py-2 px-4 rounded-xl hover:bg-blue-100 transition duration-300"
      >
        Subscribe Now
      </button>
    </form>
  </div>
</div>
