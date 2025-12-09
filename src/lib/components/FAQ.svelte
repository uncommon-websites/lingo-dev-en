<script lang="ts">
  import { slide } from 'svelte/transition';

  const faqs = [
    {
      question: "Can I switch from my translation management system?",
      answer: "Yes. Translation management systems excel at coordinating translators. Lingo.dev focuses on developer experience – automated translations happen on git push, with proper handling of variables, plurals, and UI constraints."
    },
    {
      question: "Can I switch from ChatGPT API to Lingo.dev for localization?",
      answer: "Yes, Lingo.dev is optimized for localization tasks, offering better context awareness, consistency, and integration with development workflows than raw LLM APIs."
    },
    {
      question: "How does quality assurance work with AI translations?",
      answer: "We provide tools for human review and editing. You can also configure the system to require approval for certain languages or confidence scores."
    },
    {
      question: "Can the API handle real-time chat translations?",
      answer: "Yes, our API is designed for low-latency real-time translation use cases like chat applications."
    },
    {
      question: "Does Lingo.dev work with marketing content?",
      answer: "Absolutely. Lingo.dev can handle markdown, HTML, and other content formats commonly used in marketing sites and emails."
    },
    {
      question: "How does dynamic content translation work?",
      answer: "Our SDKs allow you to pass dynamic content to the API, which returns translated strings while preserving variables and formatting."
    },
    {
      question: "How many languages does Lingo.dev support?",
      answer: "We support over 50 languages, including all major global languages and many regional dialects."
    },
    {
      question: "How secure is Lingo.dev?",
      answer: "Security is a top priority. We use enterprise-grade encryption and comply with major privacy regulations like GDPR and CCPA."
    }
  ];

  let openIndex = $state(0);
</script>

<section class="py-24 bg-gray-950 border-t border-gray-900">
  <div class="container mx-auto px-4 md:px-6">
    <h2 class="text-3xl md:text-4xl font-bold text-white mb-12">Frequently Asked Questions</h2>
    
    <div class="max-w-3xl">
      {#each faqs as faq, i}
        <div class="border-b border-gray-800">
          <button 
            class="w-full py-6 flex items-center justify-between text-left hover:text-gray-200 transition-colors focus:outline-none"
            onclick={() => openIndex = openIndex === i ? -1 : i}
          >
            <span class="text-sm font-medium {openIndex === i ? 'text-white' : 'text-gray-400'}">{faq.question}</span>
            <svg 
              class="w-4 h-4 text-gray-500 transition-transform duration-200 {openIndex === i ? 'rotate-180' : ''}" 
              viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"
            >
              <polyline points="6 9 12 15 18 9"/>
            </svg>
          </button>
          
          {#if openIndex === i}
            <div transition:slide={{ duration: 200 }}>
              <p class="pb-6 text-sm text-gray-500 leading-relaxed">
                {faq.answer}
              </p>
            </div>
          {/if}
        </div>
      {/each}
    </div>
  </div>
</section>
