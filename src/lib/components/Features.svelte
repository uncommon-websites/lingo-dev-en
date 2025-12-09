<script lang="ts">
  import Badge from './ui/Badge.svelte';
</script>

<section class="py-24 bg-gray-950 border-t border-gray-900">
  <div class="container mx-auto px-4 md:px-6">
    <div class="text-center mb-16">
      <h2 class="text-3xl md:text-4xl font-bold text-white mb-4">"Surprisingly good AI translations"</h2>
      <p class="text-gray-400 max-w-2xl mx-auto">
        Lingo.dev makes accurate localization easy: from user interfaces to dynamic content
      </p>
    </div>

    <div class="grid md:grid-cols-2 gap-6">
      <!-- Card 1: AI Localization Engine -->
      <div class="group relative overflow-hidden rounded-xl border border-gray-800 bg-[#0A0A0A] hover:border-gray-700 transition-colors">
        <div class="p-8">
          <div class="flex items-center gap-3 mb-4 text-gray-400">
            <svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M21 16V8a2 2 0 0 0-1-1.73l-7-4a2 2 0 0 0-2 0l-7 4A2 2 0 0 0 3 8v8a2 2 0 0 0 1 1.73l7 4a2 2 0 0 0 2 0l7-4A2 2 0 0 0 21 16z"/><polyline points="3.27 6.96 12 12.01 20.73 6.96"/><line x1="12" y1="22.08" x2="12" y2="12"/></svg>
            <h3 class="font-semibold text-white">AI Localization Engine</h3>
          </div>
          <p class="text-gray-400 text-sm mb-8 leading-relaxed">
            Automates translations the moment code changes are committed, ensuring high-quality results with zero manual intervention.
          </p>
          
          <div class="relative h-48 w-full flex items-center justify-center bg-[#050505] rounded-lg border border-gray-800/50 overflow-hidden">
            <!-- Grid background -->
            <div class="absolute inset-0 bg-[linear-gradient(to_right,#222_1px,transparent_1px),linear-gradient(to_bottom,#222_1px,transparent_1px)] bg-[size:20px_20px] opacity-20"></div>
            
            <!-- Chip -->
            <div class="relative z-10 w-16 h-16 bg-[#111] border border-gray-700 rounded-lg flex items-center justify-center shadow-lg shadow-primary-500/10">
              <svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="#a3e635" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="m5 12 7-7 7 7"/><path d="M12 19V5"/></svg>
              <!-- Connections -->
              <div class="absolute -left-full top-1/2 w-full h-[1px] bg-gradient-to-r from-transparent to-primary-500/50"></div>
              <div class="absolute -right-full top-1/2 w-full h-[1px] bg-gradient-to-l from-transparent to-primary-500/50"></div>
              <div class="absolute left-1/2 -top-full h-full w-[1px] bg-gradient-to-b from-transparent to-primary-500/50"></div>
              <div class="absolute left-1/2 -bottom-full h-full w-[1px] bg-gradient-to-t from-transparent to-primary-500/50"></div>
            </div>
          </div>
        </div>
      </div>

      <!-- Card 2: Git-native UI localization -->
      <div class="group relative overflow-hidden rounded-xl border border-gray-800 bg-[#0A0A0A] hover:border-gray-700 transition-colors">
        <div class="p-8">
          <div class="flex items-center gap-3 mb-4 text-gray-400">
            <svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><line x1="6" y1="3" x2="6" y2="15"/><circle cx="18" cy="6" r="3"/><circle cx="6" cy="18" r="3"/><path d="M18 9a9 9 0 0 1-9 9"/></svg>
            <h3 class="font-semibold text-white">Git-native UI localization</h3>
          </div>
          <p class="text-gray-400 text-sm mb-8 leading-relaxed">
            Localize web and mobile interfaces through Git. Automated PRs handle UI string updates in your CI/CD pipeline, keeping translations in sync.
          </p>
          
          <div class="relative h-48 w-full flex items-center justify-center bg-[#050505] rounded-lg border border-gray-800/50 overflow-hidden">
             <!-- Dashed line -->
             <div class="absolute top-1/2 left-0 w-full h-[1px] border-t border-dashed border-gray-700"></div>
             
             <!-- GitHub Icon -->
             <div class="relative z-10 w-16 h-16 bg-[#111] border border-gray-700 rounded-full flex items-center justify-center mr-12">
               <svg width="32" height="32" viewBox="0 0 24 24" fill="white"><path d="M12 0c-6.626 0-12 5.373-12 12 0 5.302 3.438 9.8 8.207 11.387.599.111.793-.261.793-.577v-2.234c-3.338.726-4.033-1.416-4.033-1.416-.546-1.387-1.333-1.756-1.333-1.756-1.089-.745.083-.729.083-.729 1.205.084 1.839 1.237 1.839 1.237 1.07 1.834 2.807 1.304 3.492.997.107-.775.418-1.305.762-1.604-2.665-.305-5.467-1.334-5.467-5.931 0-1.311.469-2.381 1.236-3.221-.124-.303-.535-1.524.117-3.176 0 0 1.008-.322 3.301 1.23.957-.266 1.983-.399 3.003-.404 1.02.005 2.047.138 3.006.404 2.291-1.552 3.297-1.23 3.297-1.23.653 1.653.242 2.874.118 3.176.77.84 1.235 1.911 1.235 3.221 0 4.609-2.807 5.624-5.479 5.921.43.372.823 1.102.823 2.222v3.293c0 .319.192.694.801.576 4.765-1.589 8.199-6.086 8.199-11.386 0-6.627-5.373-12-12-12z"/></svg>
             </div>
             
             <!-- Lingo Icon -->
             <div class="relative z-10 w-12 h-12 bg-[#111] border border-primary-500/50 rounded-lg flex items-center justify-center">
               <svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="#a3e635" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="m5 12 7-7 7 7"/><path d="M12 19V5"/></svg>
             </div>
             
             <!-- Flow animation -->
             <div class="absolute top-1/2 left-1/2 -translate-x-1/2 -translate-y-1/2 w-12 h-[1px] bg-primary-400 shadow-[0_0_10px_#a3e635]"></div>
          </div>
        </div>
      </div>

      <!-- Card 3: API & SDK -->
      <div class="group relative overflow-hidden rounded-xl border border-gray-800 bg-[#0A0A0A] hover:border-gray-700 transition-colors">
        <div class="p-8">
          <div class="flex items-center gap-3 mb-4 text-gray-400">
            <svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><polyline points="16 18 22 12 16 6"/><polyline points="8 6 2 12 8 18"/></svg>
            <h3 class="font-semibold text-white">API & SDK for dynamic content</h3>
          </div>
          <p class="text-gray-400 text-sm mb-8 leading-relaxed">
            Translate user-generated and dynamic content in real-time through our API and SDK, with built-in context awareness for accurate results.
          </p>
          
          <div class="relative w-full bg-[#050505] rounded-lg border border-gray-800/50 p-4 font-mono text-xs overflow-hidden">
            <div class="text-gray-300">
              <span class="text-purple-400">import</span> {'{'} LingoDotDevEngine {'}'} <span class="text-purple-400">from</span> <span class="text-green-400">'lingo.dev/sdk'</span>;
              <br/><br/>
              <span class="text-purple-400">const</span> <span class="text-blue-400">lingoDotDev</span> = <span class="text-purple-400">new</span> <span class="text-yellow-200">LingoDotDevEngine</span>({'{'}
              <br/>
              &nbsp;&nbsp;apiKey: <span class="text-green-400">'your-api-key-here'</span>,
              <br/>
              {'}'});
            </div>
          </div>
        </div>
      </div>

      <!-- Card 4: Customizable brand voice -->
      <div class="group relative overflow-hidden rounded-xl border border-gray-800 bg-[#0A0A0A] hover:border-gray-700 transition-colors">
        <div class="p-8">
          <div class="flex items-center gap-3 mb-4 text-gray-400">
            <svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M12 22s8-4 8-10V5l-8-3-8 3v7c0 6 8 10 8 10z"/></svg>
            <h3 class="font-semibold text-white">Customizable brand voice</h3>
          </div>
          <p class="text-gray-400 text-sm mb-8 leading-relaxed">
            Tailor translations that understand your industry's lingo and reflect your brand's unique personality, with advanced options for scaling teams.
          </p>
          
          <div class="grid grid-cols-2 gap-4">
            {#each [
              { label: 'Translation memory', on: false },
              { label: 'Formality', on: true },
              { label: 'Context Awareness', on: false },
              { label: 'Idiomic handling', on: false },
              { label: 'Content length', on: true },
              { label: 'Technical terms', on: true },
              { label: 'Gender neutrality', on: false },
              { label: 'Cultural references', on: true }
            ] as item}
              <div class="flex items-center justify-between bg-[#111] p-2 rounded border border-gray-800">
                <span class="text-xs text-gray-400">{item.label}</span>
                <div class="w-8 h-4 rounded-full relative {item.on ? 'bg-primary-500' : 'bg-gray-700'}">
                  <div class="absolute top-0.5 w-3 h-3 rounded-full bg-white transition-all {item.on ? 'left-4.5' : 'left-0.5'}"></div>
                </div>
              </div>
            {/each}
          </div>
        </div>
      </div>

      <!-- Card 5: Composable infrastructure -->
      <div class="group relative overflow-hidden rounded-xl border border-gray-800 bg-[#0A0A0A] hover:border-gray-700 transition-colors">
        <div class="p-8">
          <div class="flex items-center gap-3 mb-4 text-gray-400">
            <svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><rect x="3" y="3" width="7" height="7"/><rect x="14" y="3" width="7" height="7"/><rect x="14" y="14" width="7" height="7"/><rect x="3" y="14" width="7" height="7"/></svg>
            <h3 class="font-semibold text-white">Composable infrastructure</h3>
          </div>
          <p class="text-gray-400 text-sm mb-8 leading-relaxed">
            Full-stack localization for your product ecosystem. Translate interfaces, marketing sites, automated emails, and dynamic content seamlessly.
          </p>
          
          <div class="relative h-32 w-full flex items-center justify-center">
            <!-- Icons connected -->
            <div class="flex gap-4 items-center">
               {#each [1, 2, 3, 4] as i}
                 <div class="w-10 h-10 rounded-lg bg-[#111] border border-gray-800 flex items-center justify-center relative">
                    <div class="w-4 h-4 rounded-full bg-gray-700"></div>
                    {#if i < 4}
                      <div class="absolute -right-4 top-1/2 w-4 h-[1px] bg-gray-800"></div>
                    {/if}
                 </div>
               {/each}
            </div>
          </div>
        </div>
      </div>

      <!-- Card 6: Enterprise-grade options -->
      <div class="group relative overflow-hidden rounded-xl border border-gray-800 bg-[#0A0A0A] hover:border-gray-700 transition-colors">
        <div class="p-8">
          <div class="flex items-center gap-3 mb-4 text-gray-400">
            <svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M12 22s8-4 8-10V5l-8-3-8 3v7c0 6 8 10 8 10z"/></svg>
            <h3 class="font-semibold text-white">Enterprise-grade options</h3>
          </div>
          <p class="text-gray-400 text-sm mb-8 leading-relaxed">
            Advanced workflows, compliance features, and exceptional dedicated support with guaranteed SLAs and near-immediate response times.
          </p>
          
          <div class="relative h-32 w-full overflow-hidden rounded bg-[#050505] border border-gray-800/50">
            <!-- World Map Dots (Simplified) -->
            <div class="absolute inset-0 flex items-center justify-center opacity-30">
               <svg viewBox="0 0 200 100" class="w-full h-full text-gray-500 fill-current">
                 {#each Array(50) as _, i}
                   <circle cx={Math.random() * 200} cy={Math.random() * 100} r={Math.random() * 1.5} />
                 {/each}
               </svg>
            </div>
            <!-- Green dots -->
            <div class="absolute top-1/3 left-1/4 w-1.5 h-1.5 bg-primary-400 rounded-full shadow-[0_0_5px_#a3e635]"></div>
            <div class="absolute top-1/2 left-1/2 w-1.5 h-1.5 bg-primary-400 rounded-full shadow-[0_0_5px_#a3e635]"></div>
            <div class="absolute bottom-1/3 right-1/4 w-1.5 h-1.5 bg-primary-400 rounded-full shadow-[0_0_5px_#a3e635]"></div>
          </div>
        </div>
      </div>

    </div>
  </div>
</section>
