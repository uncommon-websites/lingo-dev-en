<script lang="ts">
  const testimonials = [
    {
      quote: "Developer experience is everything in developer tools. Lingo.dev nails it – they've turned complex localization into a few lines of code.",
      author: "Paul Copplestone",
      role: "CEO & Co-Founder, Supabase",
      logo: "⚡"
    },
    {
      quote: "With Lingo.dev, our complex fintech app is available to everyone, and we didn't need a massive team or budget to make it happen.",
      author: "Ramon Sanchez",
      role: "Co-founder, EvryThink",
      logo: "ET"
    },
    {
      quote: "Now with Lingo.dev, our engineers don't even think about localization – they just build features, and translations happen automatically in 36 languages.",
      author: "Keith Williams",
      role: "Head of Engineering, Cal.com",
      logo: "C"
    },
    {
      quote: "We tested Lingo.dev against human translations for our recruitment platform, and the AI translations were actually more accurate.",
      author: "Quentin Decré",
      role: "Co-founder, Jarvi",
      logo: "J"
    },
    {
      quote: "With Lingo.dev, Dutch reads naturally, Russian fits our UI perfectly, and our brand voice stays consistent.",
      author: "Sebastiaan van Leeuwen",
      role: "Product Manager, Truely",
      logo: "T"
    },
    {
      quote: "Lingo.dev's approach reminds me of how Stripe revolutionized payments – making a complex process invisible to developers.",
      author: "Pete Koomen",
      role: "Group Partner, Y Combinator",
      logo: "Y"
    },
    {
      quote: "With Lingo.dev, we translated 80 files instantly, and now our docs are automatically available in multiple languages.",
      author: "Iuliia Shnai",
      role: "Founder, Papermark",
      logo: "P"
    },
    {
      quote: "Before Lingo.dev, we couldn't serve our Spanish and Brazilian users well – they simply couldn't use our fintech app in their language.",
      author: "Pedro Orlando",
      role: "Co-founder, EvryThink",
      logo: "ET"
    },
    {
      quote: "Just like Dependabot made package updates effortless through automation, Lingo.dev is doing the same for localization.",
      author: "Grey Baker",
      role: "Co-founder of Dependabot",
      logo: "D"
    }
  ];
</script>

<section class="py-24 bg-gray-950 border-t border-gray-900">
  <div class="container mx-auto px-4 md:px-6">
    <div class="text-center mb-16">
      <h2 class="text-3xl md:text-4xl font-bold text-white mb-4">What developers say about Lingo.dev</h2>
      <p class="text-gray-400 max-w-2xl mx-auto">
        Join thousands of developers who trust Lingo.dev for their localization needs
      </p>
    </div>

    <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-6">
      {#each testimonials as t}
        <div class="p-6 rounded-xl border border-gray-800 bg-[#0A0A0A] hover:border-gray-700 transition-colors flex flex-col justify-between h-full">
          <p class="text-gray-300 mb-6 leading-relaxed">"{t.quote}"</p>
          
          <div class="flex items-center justify-between mt-auto">
            <div class="flex items-center gap-3">
              <div class="w-10 h-10 rounded-full bg-gray-800 flex items-center justify-center text-xs font-bold text-gray-500 overflow-hidden">
                <!-- Placeholder Avatar -->
                <svg width="24" height="24" viewBox="0 0 24 24" fill="currentColor" class="text-gray-600"><path d="M12 12c2.21 0 4-1.79 4-4s-1.79-4-4-4-4 1.79-4 4 1.79 4 4 4zm0 2c-2.67 0-8 1.34-8 4v2h16v-2c0-2.66-5.33-4-8-4z"/></svg>
              </div>
              <div>
                <div class="font-semibold text-white text-sm">{t.author}</div>
                <div class="text-xs text-gray-500">{t.role}</div>
              </div>
            </div>
            
            <div class="w-8 h-8 rounded bg-gray-900 border border-gray-800 flex items-center justify-center text-xs font-bold text-gray-400">
              {t.logo}
            </div>
          </div>
        </div>
      {/each}
    </div>
  </div>
</section>
