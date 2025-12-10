<script>
  export let active = false;
</script>

<header class="fixed top-0 left-0 w-full z-50 bg-background/80 backdrop-blur-md border-b border-white/10">
  <!-- Top Banner -->
  <div class="w-full bg-black text-xs py-2 text-center border-b border-white/10">
    <span class="text-gray-400">✦ We raised $20M at a $750M valuation ✦</span>
    <a href="#" class="text-white underline ml-2 hover:text-accent transition-colors">Read More</a>
  </div>

  <!-- Main Nav -->
  <div class="max-w-[1400px] mx-auto px-6 h-16 flex items-center justify-between">
    <!-- Logo -->
    <a href="/" class="flex items-center gap-2 group">
      <div class="w-8 h-8 border border-white/20 rounded flex items-center justify-center text-white font-bold group-hover:border-accent transition-colors">
        AI
      </div>
    </a>

    <!-- Links -->
    <nav class="hidden md:flex items-center gap-8 text-sm font-medium text-gray-400">
      <a href="#" class="hover:text-white transition-colors">Technology</a>
      <a href="#" class="hover:text-white transition-colors">Product</a>
      <a href="#" class="hover:text-white transition-colors">Pricing</a>
      <a href="#" class="hover:text-white transition-colors">Company</a>
      <a href="#" class="hover:text-white transition-colors">Blog</a>
    </nav>

    <!-- CTA -->
    <a href="#" class="bg-accent hover:bg-accent/90 text-white text-xs font-semibold px-4 py-2 rounded transition-colors">
      Apollo-1 Playground
    </a>
  </div>
</header>
