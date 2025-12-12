<script lang="ts">
	// Platform logos
	const platforms = [
		{ name: 'Windows', width: 80 },
		{ name: 'macOS', width: 90 },
		{ name: 'Linux', width: 80 },
		{ name: 'iOS', width: 60 },
		{ name: 'Android', width: 90 },
		{ name: 'WebAssembly', width: 100 }
	];
</script>

<section class="relative pt-32 pb-16 px-6 md:px-12 max-w-7xl mx-auto min-h-screen flex flex-col justify-between">
	<div class="grid grid-cols-1 lg:grid-cols-2 gap-12 items-center">
		<div class="z-10">
			<h1 class="text-6xl md:text-7xl lg:text-8xl font-display font-medium text-gray-900 leading-[0.9] tracking-tight mb-8">
				Build Native<br>
				<span class="text-brand-green">Cross-Platform</span><br>
				Apps
			</h1>
			
			<div class="relative w-12 h-12 mb-8">
				<!-- Platform icon -->
				<svg viewBox="0 0 24 24" fill="none" class="w-10 h-10 text-brand-green absolute top-0 left-0">
					<rect x="3" y="3" width="7" height="7" fill="currentColor" opacity="0.7"/>
					<rect x="14" y="3" width="7" height="7" fill="currentColor" opacity="0.5"/>
					<rect x="3" y="14" width="7" height="7" fill="currentColor" opacity="0.5"/>
					<rect x="14" y="14" width="7" height="7" fill="currentColor" opacity="0.7"/>
				</svg>
			</div>

			<div class="space-y-6 max-w-lg">
				<p class="font-mono text-sm text-gray-700 uppercase tracking-wider leading-relaxed">
					ONE C# CODEBASE FOR<br>
					WINDOWS, MACOS, LINUX,<br>
					IOS, ANDROID & WEB
				</p>

				<div class="flex flex-col items-start gap-3">
					<button class="bg-brand-green text-white px-6 py-3 rounded text-sm font-medium hover:bg-brand-green-hover transition-colors flex items-center gap-2">
						Get Started 
						<svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M5 12h14"/><path d="m12 5 7 7-7 7"/></svg>
					</button>
					<p class="text-[10px] text-gray-500 font-mono uppercase tracking-wide">
						free & open source - mit licensed
					</p>
				</div>
			</div>
		</div>

		<div class="relative h-[400px] lg:h-[600px] w-full flex items-center justify-center">
			<!-- Cross-platform illustration -->
			<div class="absolute inset-0 flex items-center justify-center">
				<div class="grid grid-cols-2 gap-8 w-full max-w-md">
					<!-- Desktop -->
					<div class="bg-white border-2 border-gray-300 rounded-lg p-4 shadow-lg transform -rotate-3 hover:rotate-0 transition-transform">
						<div class="w-full h-24 bg-gradient-to-br from-brand-green/20 to-brand-green/5 rounded"></div>
					</div>
					<!-- Mobile -->
					<div class="bg-white border-2 border-gray-300 rounded-2xl p-2 shadow-lg transform rotate-3 hover:rotate-0 transition-transform aspect-[9/16] max-h-48">
						<div class="w-full h-full bg-gradient-to-br from-brand-green/20 to-brand-green/5 rounded-lg"></div>
					</div>
					<!-- Tablet -->
					<div class="bg-white border-2 border-gray-300 rounded-lg p-3 shadow-lg transform rotate-2 hover:rotate-0 transition-transform col-span-2">
						<div class="w-full h-20 bg-gradient-to-br from-brand-green/20 to-brand-green/5 rounded"></div>
					</div>
				</div>
			</div>
		</div>
	</div>

	<div class="mt-20 border-t border-gray-300 pt-8">
		<div class="flex items-center gap-2 text-[10px] font-mono uppercase tracking-wider text-gray-600 mb-6">
			100,000+ APPS BUILT WITH AVALONIA UI. 
			<a href="/" class="text-brand-green hover:underline flex items-center gap-1">
				TRUSTED BY .NET DEVELOPERS WORLDWIDE ->
			</a>
		</div>
		
		<div class="grid grid-cols-2 md:grid-cols-6 gap-8 opacity-60">
			{#each platforms as platform}
				<div class="h-12 flex items-center justify-center border border-gray-300/50 rounded bg-gray-100/50">
					<span class="text-xs font-bold text-gray-500">{platform.name}</span>
				</div>
			{/each}
		</div>
	</div>
</section>
