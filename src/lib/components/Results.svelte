<section class="py-24 px-6 md:px-12 max-w-7xl mx-auto bg-[#EAEAE8]">
	<div class="text-center mb-16">
		<span class="font-mono text-[10px] text-gray-500 uppercase tracking-widest mb-4 block">
			[ PROVEN AT SCALE ]
		</span>
		<h2 class="font-display text-4xl md:text-5xl lg:text-6xl font-medium tracking-tight text-gray-900 mb-8">
			Trusted by developers worldwide.
		</h2>
		<button class="bg-black text-white px-5 py-2.5 rounded text-sm font-medium hover:bg-gray-800 transition-colors inline-flex items-center gap-2 font-mono uppercase tracking-wide text-xs">
			<svg xmlns="http://www.w3.org/2000/svg" width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M3 3v18h18"/><path d="m19 9-5 5-4-4-3 3"/></svg>
			View showcase
		</button>
	</div>

	<div class="grid grid-cols-1 md:grid-cols-2 gap-8">
		<!-- Chart 1 -->
		<div class="bg-[#F3F3F1] p-6 rounded-lg border border-gray-200">
			<h3 class="font-mono text-xs text-gray-500 uppercase mb-8">Apps Built with Avalonia UI</h3>
			<div class="h-64 relative flex items-end justify-center gap-16 pb-8">
				<!-- Bar 1 -->
				<div class="flex flex-col items-center gap-2 group">
					<span class="text-xs text-gray-500 font-mono mb-1 group-hover:text-gray-900">2020</span>
					<div class="w-16 bg-gray-300 rounded-t h-24 relative group-hover:bg-gray-400 transition-colors"></div>
					<span class="font-display text-xl font-medium">25K</span>
				</div>
				
				<!-- Bar 2 -->
				<div class="flex flex-col items-center gap-2 group">
					<span class="text-xs text-brand-green font-mono mb-1 font-bold">2024</span>
					<div class="w-16 bg-brand-green rounded-t h-48 relative group-hover:bg-brand-green-hover transition-colors">
                        <div class="absolute -top-8 left-1/2 -translate-x-1/2">
                            <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="currentColor" class="text-brand-green"><path d="M12 2L15 8L21 9L17 14L18 20L12 17L6 20L7 14L3 9L9 8L12 2Z"/></svg>
                        </div>
                    </div>
					<span class="font-display text-xl font-medium text-brand-green">100K+</span>
				</div>
			</div>
		</div>

		<!-- Chart 2 -->
		<div class="bg-[#F3F3F1] p-6 rounded-lg border border-gray-200">
			<h3 class="font-mono text-xs text-gray-500 uppercase mb-8">Community Growth</h3>
			<div class="h-64 relative w-full">
                <!-- Simple SVG Line Chart -->
                <svg viewBox="0 0 300 200" class="w-full h-full overflow-visible">
                    <!-- Axes -->
                    <line x1="0" y1="200" x2="300" y2="200" stroke="#ddd" stroke-width="1" />
                    <line x1="0" y1="0" x2="0" y2="200" stroke="#ddd" stroke-width="1" />
                    
                    <!-- Line: Growth curve -->
                    <path d="M0,180 Q75,160 150,100 T300,20" fill="none" stroke="oklch(0.58 0.19 250)" stroke-width="3" />
                    <text x="180" y="60" font-family="monospace" font-size="10" fill="oklch(0.58 0.19 250)" font-weight="bold">AVALONIA UI</text>
                    
                    <!-- Data points -->
                    <circle cx="0" cy="180" r="3" fill="oklch(0.58 0.19 250)" />
                    <circle cx="150" cy="100" r="3" fill="oklch(0.58 0.19 250)" />
                    <circle cx="300" cy="20" r="3" fill="oklch(0.58 0.19 250)" />
                </svg>
			</div>
            <div class="flex justify-between mt-4 text-[10px] text-gray-400 font-mono uppercase">
                <span>Time -></span>
                <span>Developers -></span>
            </div>
		</div>
	</div>
</section>
