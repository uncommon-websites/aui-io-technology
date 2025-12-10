<script>
  import Card from './Card.svelte';
</script>

<section class="py-20 px-6 max-w-[1400px] mx-auto space-y-24">
  
  <div class="text-center space-y-4 mb-20">
    <h2 class="text-4xl lg:text-5xl font-bold tracking-tight text-white uppercase">
      That's Where<br>
      <span class="text-white">Apollo-1</span> <span class="text-gray-500">Comes In</span>
    </h2>
    
    <div class="flex flex-wrap justify-center gap-2 mt-8">
      {#each ['Transparency', 'Controllability', 'Predictability', 'Tool-use', 'Fine-tuning'] as item}
        <span class="px-4 py-1 rounded-full border border-white/10 text-xs text-gray-400 uppercase tracking-wide bg-surface hover:border-white/30 transition-colors cursor-default">
          {item}
        </span>
      {/each}
    </div>
  </div>

  <div class="space-y-6">
    <!-- Card 1 -->
    <Card 
      subtitle="Transparency" 
      title="A Transparent,<br>White-Box<br>Model"
      theme="light"
    >
      <div slot="visual" class="w-full h-full relative p-6 flex items-center justify-center">
        <!-- Node Graph Visual -->
        <div class="relative w-full h-full">
           <!-- Nodes -->
           <div class="absolute top-1/4 left-1/4 w-3 h-3 bg-black rounded-full border border-white/20 z-10"></div>
           <div class="absolute top-1/2 left-1/2 w-4 h-4 bg-accent rounded-full z-10 shadow-[0_0_10px_rgba(255,51,0,0.5)]"></div>
           <div class="absolute bottom-1/4 right-1/4 w-3 h-3 bg-black rounded-full border border-white/20 z-10"></div>
           <div class="absolute top-1/3 right-1/3 w-2 h-2 bg-gray-400 rounded-full z-10"></div>
           
           <!-- Connections -->
           <svg class="absolute inset-0 w-full h-full pointer-events-none">
              <line x1="25%" y1="25%" x2="50%" y2="50%" stroke="rgba(0,0,0,0.2)" stroke-width="1" />
              <line x1="50%" y1="50%" x2="75%" y2="75%" stroke="rgba(0,0,0,0.2)" stroke-width="1" />
              <line x1="25%" y1="25%" x2="66%" y2="33%" stroke="rgba(0,0,0,0.1)" stroke-width="1" />
           </svg>
           
           <!-- Floating Label -->
           <div class="absolute bottom-4 left-4 bg-white/80 backdrop-blur text-[8px] px-2 py-1 rounded border border-black/5 shadow-sm">
              Confidence: 98.2%
           </div>
        </div>
      </div>
    </Card>

    <!-- Card 2 -->
    <Card 
      subtitle="Controllability" 
      title="An Advanced<br>Instruction<br>Environment"
      theme="light"
    >
      <div slot="visual" class="w-full h-full flex items-center justify-center p-6">
         <div class="w-full h-3/4 bg-[#1a1a1a] rounded-lg border border-white/10 p-3 font-mono text-[8px] text-gray-400 relative overflow-hidden shadow-xl">
            <div class="flex gap-1 mb-2">
               <div class="w-2 h-2 rounded-full bg-red-500/50"></div>
               <div class="w-2 h-2 rounded-full bg-yellow-500/50"></div>
               <div class="w-2 h-2 rounded-full bg-green-500/50"></div>
            </div>
            <div class="space-y-1">
               <div><span class="text-accent">const</span> agent = <span class="text-blue-400">new</span> Agent({`{`}</div>
               <div class="pl-2">mode: <span class="text-green-400">'strict'</span>,</div>
               <div class="pl-2">tools: [<span class="text-green-400">'web'</span>, <span class="text-green-400">'calc'</span>]</div>
               <div>{`}`});</div>
               <div class="mt-2 flex items-center">
                  <span class="text-accent mr-1">></span>
                  <span class="w-1.5 h-3 bg-accent animate-pulse"></span>
               </div>
            </div>
            
            <!-- Cursor Box -->
            <div class="absolute bottom-3 right-3 w-6 h-6 border border-accent/30 text-accent flex items-center justify-center rounded text-[8px]">
               C
            </div>
         </div>
      </div>
    </Card>

    <!-- Card 3 -->
    <Card 
      subtitle="Predictability" 
      title="A Structured<br>Reasoning<br>Process"
      theme="light"
    >
      <div slot="visual" class="w-full h-full relative bg-[#0a0a0a]">
         <!-- Grid lines -->
         <div class="absolute inset-0 bg-[linear-gradient(rgba(255,255,255,0.03)_1px,transparent_1px),linear-gradient(90deg,rgba(255,255,255,0.03)_1px,transparent_1px)] bg-[size:10px_10px]"></div>
         
         <div class="absolute top-4 right-4 w-2 h-2 border-t border-r border-white/20"></div>
         <div class="absolute bottom-4 left-4 w-2 h-2 border-b border-l border-white/20"></div>
         
         <div class="absolute inset-0 flex items-center justify-center">
            <div class="w-3/4 h-1/2 border-l border-white/10 pl-4 flex flex-col justify-between py-2">
               <div class="h-1 w-8 bg-white/20 rounded"></div>
               <div class="h-1 w-12 bg-white/20 rounded"></div>
               <div class="h-1 w-6 bg-white/20 rounded"></div>
            </div>
         </div>
         
         <div class="absolute bottom-4 right-4 w-8 h-8 rounded-full bg-white/10 flex items-center justify-center text-white text-xs hover:bg-white/20 transition-colors cursor-pointer">
            →
         </div>
      </div>
    </Card>

    <!-- Card 4 -->
    <Card 
      subtitle="Tool-Use" 
      title="100%<br>Successful<br>Tool-Use"
      theme="light"
    >
      <div slot="visual" class="w-full h-full bg-[#050505] relative overflow-hidden">
         <!-- Matrix-like rain or code -->
         <div class="absolute inset-0 opacity-20 flex justify-between px-4 text-[6px] font-mono text-green-500 leading-tight">
            <div class="flex flex-col gap-1">
               {#each Array(10) as _, i}
                  <span style="opacity: {Math.random()}">{Math.random().toString(36).substring(7)}</span>
               {/each}
            </div>
            <div class="flex flex-col gap-1 mt-4">
               {#each Array(10) as _, i}
                  <span style="opacity: {Math.random()}">{Math.random().toString(36).substring(7)}</span>
               {/each}
            </div>
            <div class="flex flex-col gap-1 mt-2">
               {#each Array(10) as _, i}
                  <span style="opacity: {Math.random()}">{Math.random().toString(36).substring(7)}</span>
               {/each}
            </div>
         </div>
         
         <!-- Central Visual -->
         <div class="absolute inset-0 flex items-center justify-center">
            <div class="w-16 h-16 border border-white/10 rounded flex items-center justify-center">
               <div class="w-8 h-8 bg-white/5 rotate-45"></div>
            </div>
         </div>
      </div>
    </Card>

    <!-- Card 5 -->
    <Card 
      subtitle="Fine-Tuning" 
      title="Fine-Tuning<br>Via Human<br>Feedback"
      theme="light"
    >
      <div slot="visual" class="w-full h-full bg-[#0a0a0a] flex items-center justify-center relative">
         <!-- Branching Path -->
         <svg class="w-full h-full p-8" viewBox="0 0 100 100" preserveAspectRatio="none">
            <path d="M50 100 V 50" stroke="rgba(255,255,255,0.2)" stroke-width="1" fill="none" />
            <path d="M50 50 L 20 20" stroke="rgba(255,255,255,0.2)" stroke-width="1" fill="none" />
            <path d="M50 50 L 80 20" stroke="rgba(255,255,255,0.2)" stroke-width="1" fill="none" />
            
            <!-- Nodes -->
            <circle cx="50" cy="50" r="2" fill="white" />
            <circle cx="20" cy="20" r="2" fill="#333" stroke="white" stroke-width="1" />
            <circle cx="80" cy="20" r="2" fill="#333" stroke="white" stroke-width="1" />
         </svg>
         
         <!-- Markers -->
         <div class="absolute bottom-8 left-1/2 -translate-x-1/2 w-px h-2 bg-white/20"></div>
         <div class="absolute bottom-8 left-1/3 w-px h-2 bg-white/20"></div>
         <div class="absolute bottom-8 right-1/3 w-px h-2 bg-white/20"></div>
      </div>
    </Card>
  </div>
</section>
