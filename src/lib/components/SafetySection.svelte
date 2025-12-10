<section class="py-24 px-6 max-w-[1400px] mx-auto">
  <div class="text-center mb-20">
    <h2 class="text-4xl lg:text-5xl font-bold tracking-tight text-white uppercase mb-4">
      A New Level <span class="text-gray-500">of</span><br>
      Safety & Accuracy
    </h2>
    <p class="text-gray-400 text-sm max-w-lg mx-auto">
      Combining generative and rule-based approaches minimizes the risks typically associated with AI outputs.
    </p>
  </div>

  <div class="grid grid-cols-1 lg:grid-cols-2 gap-6">
    <!-- Content Moderation -->
    <div class="lg:col-span-2 bg-surface border border-white/10 rounded-xl p-8 lg:p-12 flex flex-col lg:flex-row items-center gap-12">
      <div class="lg:w-1/3 space-y-4">
        <h3 class="text-2xl font-medium text-white">Content moderation</h3>
        <p class="text-gray-400 text-sm">
          Adheres to predefined rules to avoid generating inappropriate or harmful content.
        </p>
      </div>
      <div class="lg:w-2/3 w-full bg-black/50 border border-white/10 rounded-lg p-6 font-mono text-xs relative overflow-hidden">
         <!-- Mock Interface -->
         <div class="flex justify-between mb-4 border-b border-white/10 pb-2">
            <span class="text-white font-bold">Structured Reasoning</span>
            <span class="text-gray-500">Generic Planning</span>
         </div>
         
         <div class="space-y-3">
            <div class="flex items-start gap-3">
               <div class="w-4 h-4 rounded-full bg-red-500/20 flex items-center justify-center text-red-500 mt-0.5">!</div>
               <div>
                  <div class="text-white">Identify missing/required parameters</div>
                  <div class="text-gray-500 text-[10px] mt-1 flex gap-2">
                     <span>Product Type</span>
                     <span>Nominal Budget</span>
                     <span>Brand/Model</span>
                  </div>
               </div>
            </div>
            
            <div class="flex items-start gap-3 bg-red-500/10 p-2 rounded border border-red-500/20">
               <div class="w-4 h-4 rounded-full bg-red-500 flex items-center justify-center text-white text-[10px] mt-0.5">X</div>
               <div>
                  <div class="text-red-400">User's message blocked by 3/17 guardrails</div>
                  <div class="text-red-300/70 text-[10px]">The requested product type "illegal drugs" violates policy.</div>
               </div>
            </div>
         </div>
      </div>
    </div>

    <!-- Information Accuracy -->
    <div class="bg-surface border border-white/10 rounded-xl p-8 min-h-[300px] flex flex-col justify-between">
      <div class="mb-8">
         <h3 class="text-xl font-medium text-white mb-2">Information accuracy</h3>
         <div class="space-y-4 mt-6">
            <div class="flex items-center gap-3">
               <div class="w-6 h-6 rounded-full bg-surface-light border border-white/10 flex items-center justify-center text-xs text-gray-400">1</div>
               <div class="text-sm text-gray-300">Evaluating Company Policies Tool</div>
            </div>
            <div class="flex items-center gap-3">
               <div class="w-6 h-6 rounded-full bg-surface-light border border-white/10 flex items-center justify-center text-xs text-gray-400">2</div>
               <div class="text-sm text-gray-300">Company Policies</div>
            </div>
         </div>
      </div>
    </div>

    <!-- Auditability -->
    <div class="bg-surface border border-white/10 rounded-xl p-8 min-h-[300px] flex flex-col justify-between">
      <div class="mb-8">
         <h3 class="text-xl font-medium text-white mb-2">Auditability</h3>
         <div class="mt-6 bg-surface-light border border-white/5 rounded p-4">
            <div class="flex justify-between items-center text-xs text-gray-400 mb-2">
               <span>History Review</span>
               <span>v</span>
            </div>
            <div class="h-20 border-t border-white/5 pt-2 text-[10px] text-gray-500">
               Utterance 1: show me the user's position...
            </div>
         </div>
      </div>
    </div>
  </div>
</section>
