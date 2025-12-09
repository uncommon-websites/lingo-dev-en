<script lang="ts">
  import Button from './ui/Button.svelte';
  import Badge from './ui/Badge.svelte';
</script>

<section class="relative overflow-hidden pt-20 pb-32 md:pt-32 md:pb-48">
  <!-- Background Grid -->
  <div class="absolute inset-0 bg-[linear-gradient(to_right,#80808012_1px,transparent_1px),linear-gradient(to_bottom,#80808012_1px,transparent_1px)] bg-[size:24px_24px] [mask-image:radial-gradient(ellipse_60%_50%_at_50%_0%,#000_70%,transparent_100%)] pointer-events-none"></div>

  <div class="container mx-auto px-4 md:px-6 relative z-10">
    <div class="grid lg:grid-cols-2 gap-12 items-center">
      <div class="max-w-2xl">
        <div class="mb-8">
          <Badge class="border-orange-500/20 bg-orange-500/10 hover:bg-orange-500/20 transition-colors cursor-default">
            <span class="text-gray-400 mr-1.5">Backed by</span>
            <span class="bg-[#F26522] text-white text-[10px] font-bold px-1 py-0.5 rounded-sm mr-1.5">Y</span>
            <span class="text-white">Combinator</span>
          </Badge>
        </div>
        
        <h1 class="text-5xl md:text-7xl font-bold tracking-tight text-white mb-6 leading-[1.1]">
          Build.<br/>
          Commit.<br/>
          Translate.
        </h1>
        
        <p class="text-xl text-gray-400 mb-8 max-w-lg leading-relaxed">
          AI localization for teams that <em class="text-gray-300 not-italic">ship fast</em>. Translate apps, websites, and entire databases using the best LLM models.
        </p>
        
        <div class="flex flex-wrap items-center gap-4">
          <Button size="lg" class="bg-primary-400 hover:bg-primary-300 text-black font-semibold px-8">
            Get started
          </Button>
          <Button variant="ghost" size="lg" class="group">
            See the docs 
            <svg class="ml-2 w-4 h-4 transition-transform group-hover:translate-x-1" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M7 17L17 7"/><path d="M7 7h10v10"/></svg>
          </Button>
        </div>
      </div>

      <div class="relative hidden lg:block">
        <!-- Abstract Chip Graphic -->
        <div class="relative w-full aspect-square max-w-md mx-auto">
          <!-- Glow -->
          <div class="absolute inset-0 bg-primary-500/20 blur-[100px] rounded-full"></div>
          
          <!-- Chip Body -->
          <div class="absolute inset-0 m-auto w-48 h-48 bg-[#111] border border-gray-800 rounded-2xl shadow-2xl flex items-center justify-center z-10">
            <!-- Inner Chip -->
            <div class="w-32 h-32 bg-gray-900/80 rounded-xl border border-gray-700 flex items-center justify-center relative overflow-hidden">
               <!-- Scanline effect -->
               <div class="absolute inset-0 bg-[linear-gradient(transparent_50%,rgba(0,0,0,0.5)_50%)] bg-[size:100%_4px] opacity-20 pointer-events-none"></div>
               
               <!-- Logo -->
               <div class="relative z-10 text-primary-400">
                 <svg width="48" height="48" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="3" stroke-linecap="round" stroke-linejoin="round"><path d="m5 12 7-7 7 7"/><path d="M12 19V5"/></svg>
               </div>
            </div>
            
            <!-- Pins -->
            {#each Array(6) as _, i}
              <div class="absolute -left-3 top-1/2 -translate-y-1/2 flex flex-col gap-3" style="transform: translateY({(i-2.5)*12}px)">
                <div class="w-3 h-1 bg-gray-600 rounded-full"></div>
              </div>
              <div class="absolute -right-3 top-1/2 -translate-y-1/2 flex flex-col gap-3" style="transform: translateY({(i-2.5)*12}px)">
                <div class="w-3 h-1 bg-gray-600 rounded-full"></div>
              </div>
              <div class="absolute -top-3 left-1/2 -translate-x-1/2 flex gap-3" style="transform: translateX({(i-2.5)*12}px)">
                <div class="w-1 h-3 bg-gray-600 rounded-full"></div>
              </div>
              <div class="absolute -bottom-3 left-1/2 -translate-x-1/2 flex gap-3" style="transform: translateX({(i-2.5)*12}px)">
                <div class="w-1 h-3 bg-gray-600 rounded-full"></div>
              </div>
            {/each}
          </div>

          <!-- Circuit Lines -->
          <svg class="absolute inset-0 w-full h-full text-gray-800" viewBox="0 0 400 400" fill="none">
            <path d="M200 100 V 50 M200 300 V 350 M100 200 H 50 M300 200 H 350" stroke="currentColor" stroke-width="2" />
            <path d="M180 100 V 60 M220 100 V 60 M180 300 V 340 M220 300 V 340" stroke="currentColor" stroke-width="2" />
            <path d="M100 180 H 60 M100 220 H 60 M300 180 H 340 M300 220 H 340" stroke="currentColor" stroke-width="2" />
            
            <!-- Animated signals -->
            <circle r="2" fill="#a3e635" class="animate-ping">
              <animateMotion dur="3s" repeatCount="indefinite" path="M200 100 V 50" />
            </circle>
            <circle r="2" fill="#a3e635">
              <animateMotion dur="4s" repeatCount="indefinite" path="M100 200 H 50" />
            </circle>
          </svg>
        </div>
      </div>
    </div>
  </div>
</section>
