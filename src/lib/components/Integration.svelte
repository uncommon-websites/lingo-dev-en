<script lang="ts">
  import { fade } from 'svelte/transition';

  let activeTab = $state(0);

  const tabs = [
    {
      title: "CI/CD Integration",
      description: "Prevent incomplete releases by integrating Lingo.dev into your CI/CD pipeline.",
      link: "Learn more",
      file: "config.yml",
      code: `jobs:
  release:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v2
      - uses: actions/setup-node@v2
        with:
          node-version: "20"
      - run: npm ci
      - run: npx lingo.dev@latest i18n --frozen
      - run: npm run build
      - run: npm run deploy`
    },
    {
      title: "JavaScript SDK",
      description: "Add real-time AI-powered translations to your JavaScript applications.",
      link: "Learn more",
      file: "app.js",
      code: `import { LingoDotDev } from '@lingo.dev/sdk';

const lingo = new LingoDotDev({
  apiKey: process.env.LINGO_API_KEY
});

// Translate text in real-time
const translated = await lingo.translate(
  "Hello world", 
  "es"
);

console.log(translated); // "Hola mundo"`
    },
    {
      title: "Powerful CLI",
      description: "Translate your project with Lingo.dev's powerful CLI tool.",
      link: "Learn more",
      file: "terminal",
      code: `$ npm install -g lingo.dev

$ lingo init
> Project initialized!

$ lingo translate
> Scanning files...
> Found 120 strings
> Translating to 5 languages...
> Done! 🚀`
    }
  ];
</script>

<section class="py-24 bg-gray-950">
  <div class="container mx-auto px-4 md:px-6">
    <div class="text-center mb-16">
      <h2 class="text-3xl md:text-4xl font-bold text-white mb-4">Integrate as you want</h2>
      <p class="text-gray-400 max-w-2xl mx-auto">
        Lingo.dev integrates with your existing tools and workflows to make localization easy
      </p>
    </div>

    <div class="grid lg:grid-cols-12 gap-8 items-start">
      <!-- Tabs -->
      <div class="lg:col-span-4 flex flex-col gap-2">
        {#each tabs as tab, i}
          <button 
            class="text-left p-6 rounded-xl transition-all duration-300 border border-transparent {activeTab === i ? 'bg-[#111] border-gray-800' : 'hover:bg-gray-900/50'}"
            onclick={() => activeTab = i}
          >
            <div class="flex items-center gap-3 mb-2">
              <div class="h-full w-0.5 bg-primary-400 rounded-full transition-all duration-300 {activeTab === i ? 'h-4 opacity-100' : 'h-0 opacity-0'}"></div>
              <h3 class="font-semibold text-lg {activeTab === i ? 'text-primary-400' : 'text-gray-300'}">
                {tab.title}
              </h3>
            </div>
            <p class="text-sm text-gray-400 mb-4 pl-3.5 leading-relaxed">
              {tab.description}
            </p>
            <div class="pl-3.5 flex items-center text-sm font-medium text-gray-500 hover:text-white transition-colors">
              {tab.link} 
              <svg class="ml-1 w-3 h-3" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M7 17L17 7"/><path d="M7 7h10v10"/></svg>
            </div>
          </button>
        {/each}
      </div>

      <!-- Code Block -->
      <div class="lg:col-span-8">
        <div class="relative rounded-xl overflow-hidden bg-[#0A0A0A] border border-gray-800 shadow-2xl">
          <!-- Window Controls -->
          <div class="flex items-center justify-between px-4 py-3 border-b border-gray-800 bg-[#111]">
            <span class="text-xs font-mono text-gray-400">{tabs[activeTab].file}</span>
            <button class="text-gray-500 hover:text-white transition-colors">
              <svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><rect x="9" y="9" width="13" height="13" rx="2" ry="2"/><path d="M5 15H4a2 2 0 0 1-2-2V4a2 2 0 0 1 2-2h9a2 2 0 0 1 2 2v1"/></svg>
            </button>
          </div>
          
          <!-- Code -->
          <div class="p-6 overflow-x-auto">
            {#key activeTab}
              <pre class="font-mono text-sm leading-relaxed" in:fade={{ duration: 200 }}>
                {#each tabs[activeTab].code.split('\n') as line, i}
                  <div class="table-row">
                    <span class="table-cell text-gray-700 select-none pr-4 text-right w-8">{i + 1}</span>
                    <span class="table-cell">
                      {@html line
                        .replace(/jobs:|release:|steps:|runs-on:|uses:|with:|run:/g, '<span class="text-primary-400">$&</span>')
                        .replace(/npm|npx/g, '<span class="text-blue-400">$&</span>')
                        .replace(/"[^"]*"/g, '<span class="text-orange-300">$&</span>')
                        .replace(/import|from|const|await|new/g, '<span class="text-purple-400">$&</span>')
                        .replace(/\/\/.*/g, '<span class="text-gray-500">$&</span>')
                      }
                    </span>
                  </div>
                {/each}
              </pre>
            {/key}
          </div>
        </div>
      </div>
    </div>
  </div>
</section>
