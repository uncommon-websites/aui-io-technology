<section class="relative pt-32 pb-20 px-6 max-w-[1400px] mx-auto min-h-[80vh] flex flex-col justify-center">
  <div class="grid grid-cols-1 lg:grid-cols-2 gap-12 items-center">
    <!-- Left Content -->
    <div class="space-y-8">
      <h1 class="text-5xl lg:text-7xl font-bold tracking-tight leading-[0.9] text-white">
        <span class="text-accent">APOLLO-1:</span><br>
        THE NEURO-SYMBOLIC<br>
        FOUNDATION MODEL <span class="text-gray-400 font-normal">THAT</span><br>
        <span class="text-gray-400 font-normal">SOLVES TASK-ORIENTED</span><br>
        <span class="text-gray-400 font-normal">CONVERSATIONAL AI</span>
      </h1>
      
      <button class="bg-white text-black px-6 py-3 rounded font-medium hover:bg-gray-200 transition-colors">
        Read Blog
      </button>
    </div>

    <!-- Right Content (Diagram) -->
    <div class="relative bg-surface border border-white/10 rounded-xl p-6 lg:p-10 w-full aspect-video flex flex-col items-center justify-center overflow-hidden">
      <!-- Diagram Title -->
      <div class="absolute top-6 left-0 w-full text-center text-gray-400 text-xs uppercase tracking-widest">
        Apollo-1's Neuro-Symbolic Reasoner
      </div>

      <!-- Diagram Container -->
      <div class="flex flex-col items-center gap-4 w-full max-w-lg mt-8 text-[10px] text-gray-300">
        
        <!-- Top Row -->
        <div class="flex items-center justify-center gap-2 w-full">
           <div class="border border-white/20 rounded px-2 py-1 bg-surface-light">System prompts</div>
        </div>

        <!-- Middle Flow -->
        <div class="flex items-center justify-between w-full gap-2">
          <div class="flex flex-col items-center gap-1">
             <div class="border border-white/20 rounded px-3 py-2 bg-surface-light">User Input</div>
             <div class="h-4 w-px bg-white/20"></div>
             <div class="border border-accent/50 text-accent rounded px-3 py-2 bg-accent/10">Neural Symbolic<br>Encoder</div>
          </div>

          <div class="h-px w-8 bg-white/20"></div>

          <div class="flex flex-col items-center gap-1 flex-1 border border-dashed border-white/20 rounded p-2">
             <div class="text-[8px] text-gray-500 mb-1">Reasoning Engine</div>
             <div class="flex gap-2">
                <div class="border border-white/20 rounded px-2 py-1 bg-surface-light">Symbolic<br>Logic</div>
                <div class="border border-white/20 rounded px-2 py-1 bg-surface-light">Neural<br>Planner</div>
             </div>
          </div>

          <div class="h-px w-8 bg-white/20"></div>

          <div class="flex flex-col items-center gap-1">
             <div class="border border-accent/50 text-accent rounded px-3 py-2 bg-accent/10">Symbolic<br>Decoder</div>
             <div class="h-4 w-px bg-white/20"></div>
             <div class="border border-white/20 rounded px-3 py-2 bg-surface-light">Model<br>Output</div>
          </div>
        </div>

        <!-- Bottom Flow -->
        <div class="flex items-center gap-4 mt-2">
           <div class="h-8 w-px bg-white/20"></div>
        </div>
        <div class="flex items-center gap-4">
           <div class="border border-white/20 rounded px-3 py-2 bg-surface-light">Tool invocation</div>
           <div class="w-8 h-px bg-white/20"></div>
           <div class="border border-white/20 rounded px-3 py-2 bg-surface-light">External endpoints<br>(API/DB/SCRIPTS)</div>
        </div>

      </div>
      
      <!-- Background Grid/Decor -->
      <div class="absolute inset-0 bg-[linear-gradient(rgba(255,255,255,0.03)_1px,transparent_1px),linear-gradient(90deg,rgba(255,255,255,0.03)_1px,transparent_1px)] bg-[size:20px_20px] pointer-events-none"></div>
    </div>
  </div>
  
  <!-- Corner markers -->
  <div class="absolute top-24 left-6 w-2 h-2 border-t border-l border-white/30"></div>
  <div class="absolute top-24 right-6 w-2 h-2 border-t border-r border-white/30"></div>
  <div class="absolute bottom-10 left-6 w-2 h-2 border-b border-l border-white/30"></div>
  <div class="absolute bottom-10 right-6 w-2 h-2 border-b border-r border-white/30"></div>
</section>
