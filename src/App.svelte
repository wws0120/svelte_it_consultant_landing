<script>
  import Hero from './components/Hero.svelte';
  import About from './components/About.svelte';
  import About2 from './components/About2.svelte';
  import About3 from './components/About3.svelte';
  import About4 from './components/About4.svelte';
  import ServicesOverview from './components/ServicesOverview.svelte';
  import Services from './components/Services.svelte';

  import Conversion from './components/Conversion.svelte';

  import FaQs from './components/FAQs.svelte';

  import Testimonials from './components/Testimonials.svelte';
  import Events from './components/Events.svelte';
  import Contact from './components/Contact.svelte';

  import Team from './components/Team.svelte';

  import WorkingProcess from './components/WorkingProcess.svelte';
  import SubscriptionSection from './components/SubscriptionSection.svelte';
  import Footer from './components/Footer.svelte';
</script>

<main class="">
  <Hero />
  <About />
  <About2 />
  <About3 />
  <About4 />
  <ServicesOverview />
  <Services />
  <WorkingProcess />
  <Team />
  <Testimonials />
  <FaQs />
  <Conversion />
  <Events />
  <SubscriptionSection />
  <Contact />
  <Footer />
</main>

<style global>
  @tailwind base;
  @tailwind components;
  @tailwind utilities;
</style>
