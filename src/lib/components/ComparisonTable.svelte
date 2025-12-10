<section class="py-20 px-6 max-w-[1400px] mx-auto">
  <div class="relative rounded-2xl overflow-hidden border border-white/10 bg-surface">
    <!-- Background Gradient -->
    <div class="absolute inset-0 opacity-30">
        <div class="absolute bottom-0 left-0 w-full h-full bg-[radial-gradient(circle_at_50%_100%,#ff4d00_0%,transparent_50%)] blur-3xl"></div>
    </div>
    
    <!-- Table Header -->
    <div class="grid grid-cols-3 border-b border-white/10 bg-white/5 backdrop-blur-sm relative z-10">
      <div class="p-6 text-xs font-mono uppercase tracking-widest text-gray-400">Feature</div>
      <div class="p-6 text-xs font-mono uppercase tracking-widest text-gray-400 border-l border-white/10">Traditional LLM Agents</div>
      <div class="p-6 text-xs font-mono uppercase tracking-widest text-black bg-white border-l border-white/10">Apollo-1 Neuro-Symbolic Agents</div>
    </div>

    <!-- Rows -->
    <div class="relative z-10">
      {#each [
        { name: 'Transparency', llm: 'Black-box model with opaque reasoning', apollo: 'White-box model with transparent reasoning processes', highlight: true },
        { name: 'Controllability', llm: 'System prompts are the primary control mechanism', apollo: 'Control levers are available throughout the system', highlight: false },
        { name: 'Predictability', llm: 'Outcomes are often unpredictable', apollo: 'Outcomes are nearly deterministic', highlight: false },
        { name: 'Tool Use', llm: 'Struggles with consistently generating structured outputs e.g. JSON', apollo: 'Tool-native with 100% success rate', highlight: false },
        { name: 'Fine-tuning', llm: 'Fine-tuning for agents is challenging', apollo: 'Supports continuous fine-tuning, even on fine-tuned models', highlight: false }
      ] as row, i}
        <div class="grid grid-cols-3 border-b border-white/10 last:border-0 hover:bg-white/5 transition-colors group">
          <div class="p-6 flex items-center gap-2 text-sm font-medium text-white">
             <span class="text-accent text-xs">///</span> {row.name}
          </div>
          <div class="p-6 text-sm text-gray-400 border-l border-white/10 flex items-center">
             {row.llm}
          </div>
          <div class="p-6 text-sm text-white font-medium border-l border-white/10 flex items-center relative overflow-hidden">
             {#if row.highlight}
               <div class="absolute inset-0 bg-white/10"></div>
             {/if}
             <span class="relative z-10">{row.apollo}</span>
          </div>
        </div>
      {/each}
    </div>
  </div>
</section>
