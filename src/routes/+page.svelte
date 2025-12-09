<script lang="ts">
  import Header from "$lib/components/Header.svelte";
  import Hero from "$lib/components/Hero.svelte";
  import Logos from "$lib/components/Logos.svelte";
  import Integration from "$lib/components/Integration.svelte";
  import Features from "$lib/components/Features.svelte";
  import Testimonials from "$lib/components/Testimonials.svelte";
  import Pricing from "$lib/components/Pricing.svelte";
  import FAQ from "$lib/components/FAQ.svelte";
  import Footer from "$lib/components/Footer.svelte";
</script>

<div class="min-h-screen bg-gray-950 text-gray-50 font-sans selection:bg-primary-500/30">
  <Header />
  
  <main>
    <Hero />
    <Logos />
    <Integration />
    <Features />
    <Testimonials />
    <Pricing />
    <FAQ />
  </main>
  
  <Footer />
</div>

