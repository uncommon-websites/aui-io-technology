<script>
  export let title = "";
  export let subtitle = "";
  export let description = "";
  export let image = ""; // Placeholder for now
  export let index = 0;
  export let theme = "light"; // 'light' or 'dark'
  
  const isDark = theme === 'dark';
</script>

<div class="group relative w-full rounded-2xl overflow-hidden border border-white/10 transition-all duration-500 hover:border-white/20">
  <div class="grid grid-cols-1 lg:grid-cols-2 min-h-[400px]">
    
    <!-- Left Content -->
    <div class={`relative p-10 flex flex-col justify-between ${isDark ? 'bg-surface' : 'bg-beige'} transition-colors`}>
      <!-- Background Gradient Effect -->
      {#if !isDark}
        <div class="absolute inset-0 bg-[radial-gradient(circle_at_100%_100%,#ff4d00_0%,transparent_50%),radial-gradient(circle_at_0%_100%,#0066ff_0%,transparent_30%)] opacity-20 blur-3xl"></div>
      {/if}

      <div class="relative z-10">
        <div class="text-[10px] font-mono uppercase tracking-widest mb-4 opacity-60" class:text-black={!isDark} class:text-white={isDark}>
          {subtitle}
        </div>
        <h3 class="text-4xl font-light tracking-tight leading-[1.1] uppercase" class:text-black={!isDark} class:text-white={isDark}>
          {@html title}
        </h3>
      </div>

      <div class="relative z-10 mt-12">
        <button class="w-8 h-8 flex items-center justify-center border rounded transition-colors" 
          class:border-black={!isDark} class:text-black={!isDark} class:hover:bg-black={!isDark} class:hover:text-white={!isDark}
          class:border-white={isDark} class:text-white={isDark} class:hover:bg-white={isDark} class:hover:text-black={isDark}>
          <span class="text-lg leading-none">+</span>
        </button>
      </div>
    </div>

    <!-- Right Content (Visual) -->
    <div class={`relative p-10 flex items-center justify-center ${isDark ? 'bg-surface-light' : 'bg-white'} border-l border-white/5`}>
      <!-- Placeholder for the interactive visual component -->
      <div class="w-full aspect-square max-w-sm bg-black rounded border border-white/10 relative overflow-hidden shadow-2xl">
        <!-- Grid Background -->
        <div class="absolute inset-0 bg-[linear-gradient(rgba(255,255,255,0.05)_1px,transparent_1px),linear-gradient(90deg,rgba(255,255,255,0.05)_1px,transparent_1px)] bg-[size:20px_20px]"></div>
        
        <!-- Content Specific to the card type -->
        <slot name="visual"></slot>
      </div>
    </div>
  </div>
</div>
