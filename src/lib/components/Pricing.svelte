<script lang="ts">
  import Button from './ui/Button.svelte';
</script>

<section class="py-24 bg-gray-950 border-t border-gray-900">
  <div class="container mx-auto px-4 md:px-6">
    <div class="text-center mb-16">
      <h2 class="text-3xl md:text-4xl font-bold text-white mb-4">10,000 words for free every month</h2>
      <p class="text-gray-400 max-w-2xl mx-auto">
        Set up for free, scale up, invite your team, and go global
      </p>
    </div>

    <div class="grid md:grid-cols-2 lg:grid-cols-4 gap-6">
      <!-- Hobby -->
      <div class="p-6 rounded-xl border border-gray-800 bg-[#0A0A0A] flex flex-col">
        <h3 class="text-lg font-semibold text-white mb-2">Hobby</h3>
        <div class="text-3xl font-bold text-white mb-1">Free</div>
        <p class="text-xs text-gray-500 mb-6">Explore the possibilities of translations on Lingo.</p>
        
        <Button variant="outline" class="w-full mb-8">Get started</Button>
        
        <ul class="space-y-3 text-sm text-gray-400 flex-1">
          <li class="flex gap-2">
            <svg class="w-4 h-4 text-gray-500 shrink-0 mt-0.5" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><polyline points="20 6 9 17 4 12"/></svg>
            10,000 translated words included monthly
          </li>
          <li class="flex gap-2">
            <svg class="w-4 h-4 text-gray-500 shrink-0 mt-0.5" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><polyline points="20 6 9 17 4 12"/></svg>
            Brand Voice & Context awareness
          </li>
          <li class="flex gap-2">
            <svg class="w-4 h-4 text-gray-500 shrink-0 mt-0.5" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><polyline points="20 6 9 17 4 12"/></svg>
            Unlimited glossary & languages
          </li>
          <li class="flex gap-2">
            <svg class="w-4 h-4 text-gray-500 shrink-0 mt-0.5" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><polyline points="20 6 9 17 4 12"/></svg>
            CI/CD integrations
          </li>
          <li class="flex gap-2">
            <svg class="w-4 h-4 text-gray-500 shrink-0 mt-0.5" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><polyline points="20 6 9 17 4 12"/></svg>
            Web & Mobile Apps
          </li>
          <li class="flex gap-2">
            <svg class="w-4 h-4 text-gray-500 shrink-0 mt-0.5" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><polyline points="20 6 9 17 4 12"/></svg>
            1 project
          </li>
        </ul>
      </div>

      <!-- Pro -->
      <div class="p-6 rounded-xl border border-primary-500/50 bg-[#0A0A0A] flex flex-col relative shadow-[0_0_20px_rgba(163,230,53,0.05)]">
        <h3 class="text-lg font-semibold text-white mb-2">Pro</h3>
        <div class="text-3xl font-bold text-white mb-1">$30 <span class="text-sm font-normal text-gray-500">/ per month</span></div>
        <p class="text-xs text-gray-500 mb-6">Build, translate, launch, and scale your apps.</p>
        
        <Button class="w-full mb-8 bg-primary-400 hover:bg-primary-300 text-black border-0">Get started</Button>
        
        <ul class="space-y-3 text-sm text-gray-400 flex-1">
          <li class="flex gap-2">
            <svg class="w-4 h-4 text-primary-400 shrink-0 mt-0.5" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M7 17L17 7"/><path d="M7 7h10v10"/></svg>
            <span class="text-white">Everything in Hobby</span>
          </li>
          <li class="flex gap-2">
            <svg class="w-4 h-4 text-gray-500 shrink-0 mt-0.5" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><polyline points="20 6 9 17 4 12"/></svg>
            20,000 translated words included monthly
          </li>
          <li class="flex gap-2">
            <svg class="w-4 h-4 text-gray-500 shrink-0 mt-0.5" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><polyline points="20 6 9 17 4 12"/></svg>
            $2.50 per additional 1,000 translated words
          </li>
          <li class="flex gap-2">
            <svg class="w-4 h-4 text-gray-500 shrink-0 mt-0.5" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><polyline points="20 6 9 17 4 12"/></svg>
            Priority email support
          </li>
        </ul>
      </div>

      <!-- Team -->
      <div class="p-6 rounded-xl border border-gray-800 bg-[#0A0A0A] flex flex-col">
        <h3 class="text-lg font-semibold text-white mb-2">Team</h3>
        <div class="text-3xl font-bold text-white mb-1">$600 <span class="text-sm font-normal text-gray-500">/ per month</span></div>
        <p class="text-xs text-gray-500 mb-6">Bring the power of Lingo to your entire team.</p>
        
        <Button variant="outline" class="w-full mb-8">Get started</Button>
        
        <ul class="space-y-3 text-sm text-gray-400 flex-1">
          <li class="flex gap-2">
            <svg class="w-4 h-4 text-white shrink-0 mt-0.5" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M7 17L17 7"/><path d="M7 7h10v10"/></svg>
            <span class="text-white">Everything in Pro</span>
          </li>
          <li class="flex gap-2">
            <svg class="w-4 h-4 text-gray-500 shrink-0 mt-0.5" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><polyline points="20 6 9 17 4 12"/></svg>
            100,000 translated words included monthly
          </li>
          <li class="flex gap-2">
            <svg class="w-4 h-4 text-gray-500 shrink-0 mt-0.5" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><polyline points="20 6 9 17 4 12"/></svg>
            $0.25 per additional 1,000 translated words
          </li>
          <li class="flex gap-2">
            <svg class="w-4 h-4 text-gray-500 shrink-0 mt-0.5" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><polyline points="20 6 9 17 4 12"/></svg>
            Unlimited projects
          </li>
          <li class="flex gap-2">
            <svg class="w-4 h-4 text-gray-500 shrink-0 mt-0.5" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><polyline points="20 6 9 17 4 12"/></svg>
            Private Slack channel
          </li>
          <li class="flex gap-2">
            <svg class="w-4 h-4 text-gray-500 shrink-0 mt-0.5" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><polyline points="20 6 9 17 4 12"/></svg>
            Web editor
          </li>
          <li class="flex gap-2">
            <svg class="w-4 h-4 text-gray-500 shrink-0 mt-0.5" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><polyline points="20 6 9 17 4 12"/></svg>
            Integrations
          </li>
        </ul>
      </div>

      <!-- Enterprise -->
      <div class="p-6 rounded-xl border border-gray-800 bg-[#0A0A0A] flex flex-col">
        <h3 class="text-lg font-semibold text-white mb-2">Enterprise</h3>
        <div class="text-3xl font-bold text-white mb-1">Custom</div>
        <p class="text-xs text-gray-500 mb-6">Scale securely with enterprise-grade compliance and premium support.</p>
        
        <Button variant="outline" class="w-full mb-8">Contact us</Button>
        
        <ul class="space-y-3 text-sm text-gray-400 flex-1">
          <li class="flex gap-2">
            <svg class="w-4 h-4 text-white shrink-0 mt-0.5" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M7 17L17 7"/><path d="M7 7h10v10"/></svg>
            <span class="text-white">Everything on Team plan</span>
          </li>
          <li class="flex gap-2">
            <svg class="w-4 h-4 text-gray-500 shrink-0 mt-0.5" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><polyline points="20 6 9 17 4 12"/></svg>
            Custom word volume
          </li>
          <li class="flex gap-2">
            <svg class="w-4 h-4 text-gray-500 shrink-0 mt-0.5" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><polyline points="20 6 9 17 4 12"/></svg>
            SLAs
          </li>
          <li class="flex gap-2">
            <svg class="w-4 h-4 text-gray-500 shrink-0 mt-0.5" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><polyline points="20 6 9 17 4 12"/></svg>
            Dedicated support
          </li>
        </ul>
      </div>
    </div>
  </div>
</section>
