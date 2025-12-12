<script lang="ts">
	import FeatureCard from './FeatureCard.svelte';
</script>

<section class="py-24 px-6 md:px-12 max-w-7xl mx-auto relative" id="features">
    <!-- Background Grid Pattern -->
    <div class="absolute inset-0 z-0 opacity-30 pointer-events-none" 
        style="background-image: linear-gradient(#ccc 1px, transparent 1px), linear-gradient(90deg, #ccc 1px, transparent 1px); background-size: 40px 40px; mask-image: linear-gradient(to bottom, transparent, black 10%, black 90%, transparent);">
    </div>

	<div class="flex flex-col md:flex-row justify-between items-start md:items-end mb-16 gap-6 relative z-10">
		<div>
			<span class="font-mono text-[10px] text-gray-500 uppercase tracking-widest mb-4 block">
				[ POWERFUL FEATURES ]
			</span>
			<h2 class="font-display text-4xl md:text-5xl lg:text-6xl font-medium tracking-tight text-gray-900 mb-4">
				Everything you need.
			</h2>
			<p class="font-mono text-sm text-gray-600 max-w-lg">
				Avalonia UI provides a complete toolkit for building modern, native desktop applications.
			</p>
		</div>
		
		<button class="bg-black text-white px-5 py-2.5 rounded text-sm font-medium hover:bg-gray-800 transition-colors flex items-center gap-2 font-mono uppercase tracking-wide text-xs">
			View Documentation ->
		</button>
	</div>

	<div class="grid grid-cols-1 md:grid-cols-2 gap-6">
		<FeatureCard 
			subtitle="[ CROSS-PLATFORM ]"
			title="Write once,<br>run everywhere"
			description="Single C# codebase deploys to Windows, macOS, Linux, iOS, Android, and WebAssembly."
			tagColor="bg-brand-green"
			tagIcon="arrow"
            imageSrc="https://placehold.co/600x400/FFFFFF/E5E7EB?text=Cross+Platform"
		/>
		
		<FeatureCard 
			subtitle="[ FAMILIAR XAML ]"
			title="Use the tools<br>you already know"
			description="Leverage your existing XAML knowledge with a syntax familiar to WPF and UWP developers."
			tagColor="bg-accent-orange"
			tagIcon="plus"
            imageSrc="https://placehold.co/600x400/FFFFFF/E5E7EB?text=XAML+Editor"
		/>
		
		<FeatureCard 
			subtitle="[ NATIVE PERFORMANCE ]"
			title="Fast, responsive<br>native applications"
			description="Hardware-accelerated rendering delivers smooth 60fps experiences on every platform."
			tagColor="bg-accent-pink"
			tagIcon="arrow"
            imageSrc="https://placehold.co/600x400/FFFFFF/E5E7EB?text=Performance"
		/>
		
		<FeatureCard 
			subtitle="[ RICH CONTROLS ]"
			title="Complete UI toolkit<br>out of the box"
			description="Extensive library of controls, styles, and themes to build beautiful applications quickly."
			tagColor="bg-accent-yellow"
			tagIcon="plus"
            imageSrc="https://placehold.co/600x400/FFFFFF/E5E7EB?text=UI+Controls"
		/>
	</div>
</section>
