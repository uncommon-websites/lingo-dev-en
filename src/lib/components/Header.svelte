<script lang="ts">
  import Button from './ui/Button.svelte';
</script>

<div class="w-full bg-primary-400 text-black text-center text-xs font-medium py-1.5 px-4">
  <span class="inline-flex items-center gap-1">
    <svg width="12" height="12" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="animate-pulse"><path d="m12 3-1.912 5.813a2 2 0 0 1-1.275 1.275L3 12l5.813 1.912a2 2 0 0 1 1.275 1.275L12 21l1.912-5.813a2 2 0 0 1 1.275-1.275L21 12l-5.813-1.912a2 2 0 0 1-1.275-1.275L12 3Z"/></svg>
    Big update launching soon. <a href="#" class="underline decoration-black/30 hover:decoration-black">Join the early access list</a>
  </span>
</div>

<header class="sticky top-0 z-50 w-full border-b border-gray-800 bg-gray-950/80 backdrop-blur-md">
  <div class="container mx-auto flex h-16 items-center justify-between px-4 md:px-6">
    <div class="flex items-center gap-8">
      <a href="/" class="flex items-center gap-2 font-bold text-xl tracking-tight">
        <div class="relative flex h-6 w-6 items-center justify-center rounded bg-primary-400 text-black">
          <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="3" stroke-linecap="round" stroke-linejoin="round"><path d="m5 12 7-7 7 7"/><path d="M12 19V5"/></svg>
        </div>
        Lingo.dev
      </a>
      
      <nav class="hidden md:flex items-center gap-6 text-sm font-medium text-gray-400">
        <a href="#" class="hover:text-white transition-colors">Get started</a>
        <a href="#" class="hover:text-white transition-colors">CLI</a>
        <a href="#" class="hover:text-white transition-colors">CI/CD</a>
        <a href="#" class="hover:text-white transition-colors">SDK</a>
        <a href="#" class="flex items-center gap-1.5 hover:text-white transition-colors">
          MCP 
          <span class="rounded bg-primary-400/10 px-1.5 py-0.5 text-[10px] uppercase leading-none text-primary-400">new</span>
        </a>
        <a href="#" class="flex items-center gap-1.5 hover:text-white transition-colors">
          Compiler
          <span class="rounded bg-yellow-500/10 px-1.5 py-0.5 text-[10px] uppercase leading-none text-yellow-500">exp</span>
        </a>
      </nav>
    </div>

    <div class="flex items-center gap-4">
      <div class="hidden sm:flex items-center gap-4 text-sm text-gray-400">
        <button class="hover:text-white transition-colors">en</button>
        <a href="#" class="flex items-center gap-1 hover:text-white transition-colors">
          <svg width="16" height="16" viewBox="0 0 24 24" fill="currentColor" stroke="none"><path d="M12 2C6.477 2 2 6.477 2 12c0 4.42 2.87 8.17 6.84 9.5.5.08.66-.23.66-.5v-1.69c-2.77.6-3.36-1.34-3.36-1.34-.46-1.16-1.11-1.47-1.11-1.47-.91-.62.07-.6.07-.6 1 .07 1.53 1.03 1.53 1.03.87 1.52 2.34 1.07 2.91.83.09-.65.35-1.09.63-1.34-2.22-.25-4.55-1.11-4.55-4.92 0-1.11.38-2 1.03-2.71-.1-.25-.45-1.29.1-2.64 0 0 .84-.27 2.75 1.02.79-.22 1.65-.33 2.5-.33.85 0 1.71.11 2.5.33 1.91-1.29 2.75-1.02 2.75-1.02.55 1.35.2 2.39.1 2.64.65.71 1.03 1.6 1.03 2.71 0 3.82-2.34 4.66-4.57 4.91.36.31.69.92.69 1.85V21c0 .27.16.59.67.5C19.14 20.16 22 16.42 22 12A10 10 0 0 0 12 2Z"/></svg>
          <span class="text-xs">5.0k</span>
        </a>
        <button class="hover:text-white transition-colors">
          <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><circle cx="12" cy="12" r="4"/><path d="M12 2v2"/><path d="M12 20v2"/><path d="m4.93 4.93 1.41 1.41"/><path d="m17.66 17.66 1.41 1.41"/><path d="M2 12h2"/><path d="M20 12h2"/><path d="m6.34 17.66-1.41 1.41"/><path d="m19.07 4.93-1.41 1.41"/></svg>
        </button>
      </div>
      
      <Button variant="secondary" size="sm" class="hidden sm:inline-flex">Platform</Button>
    </div>
  </div>
</header>
