<script lang="ts">
	const testimonials = [
		{
			quote: "Avalonia UI has been a game-changer for our desktop application. We went from maintaining three separate codebases to just one, and the performance is incredible.",
			author: "Sarah Chen",
			role: "Lead Developer • TechCorp",
			image: "https://i.pravatar.cc/150?u=sarah",
            icon: "https://placehold.co/20x20/333/fff?text=T"
		},
		{
			quote: "The XAML syntax feels so familiar coming from WPF. We were able to port our entire application in weeks, not months. Avalonia UI is the future of .NET desktop development.",
			author: "Michael Rodriguez",
			role: "Senior Engineer • DataFlow Systems",
			image: "https://i.pravatar.cc/150?u=michael",
            icon: "https://placehold.co/20x20/000/fff?text=D"
		},
		{
			quote: "Cross-platform development that actually works. Our app runs beautifully on Windows, Mac, and Linux with native performance on each platform.",
			author: "Emma Thompson",
			role: "CTO • CloudSync",
			image: "https://i.pravatar.cc/150?u=emma",
            icon: "https://placehold.co/20x20/purple/fff?text=C"
		},
		{
			quote: "The community support is outstanding. Every question I've had has been answered quickly, and the documentation keeps getting better.",
			author: "David Kim",
			role: "Indie Developer",
			image: "https://i.pravatar.cc/150?u=david",
            icon: "https://placehold.co/20x20/blue/fff?text=D"
		},
		{
			quote: "We chose Avalonia UI for our enterprise application and haven't looked back. The MVVM support and data binding make complex UIs manageable.",
			author: "Lisa Martinez",
			role: "Tech Lead • Enterprise Solutions Inc",
			image: "https://i.pravatar.cc/150?u=lisa",
            icon: "https://placehold.co/20x20/green/fff?text=E"
		},
		{
			quote: "Finally, a truly cross-platform UI framework that doesn't compromise on performance or developer experience. Avalonia UI is what .NET developers have been waiting for.",
			author: "James Wilson",
			role: "Software Architect • DevTools Pro",
			image: "https://i.pravatar.cc/150?u=james",
            icon: "https://placehold.co/20x20/red/fff?text=D"
		},
        {
			quote: "The hot reload feature has dramatically improved our development workflow. We can see changes instantly across all platforms.",
			author: "Rachel Green",
			role: "UI Developer • DesignFirst",
			image: "https://i.pravatar.cc/150?u=rachel",
            icon: "https://placehold.co/20x20/333/fff?text=D"
		},
        {
			quote: "Avalonia UI's rendering performance is exceptional. Our data visualization app handles thousands of elements smoothly at 60fps.",
			author: "Alex Patel",
			role: "Principal Engineer • DataViz Labs",
			image: "https://i.pravatar.cc/150?u=alex",
            icon: "https://placehold.co/20x20/orange/fff?text=D"
		}
	];
</script>

<section class="py-24 px-6 md:px-12 max-w-7xl mx-auto">
	<div class="text-center mb-16">
		<span class="font-mono text-[10px] text-gray-500 uppercase tracking-widest mb-4 block">
			[ TESTIMONIALS ]
		</span>
		<h2 class="font-display text-4xl md:text-5xl font-medium tracking-tight text-gray-900 mb-4">
			Loved by .NET Developers
		</h2>
		<p class="font-mono text-sm text-gray-600">
			See what developers are saying about building with Avalonia UI
		</p>
	</div>

	<div class="columns-1 md:columns-2 lg:columns-3 gap-6 space-y-6">
		{#each testimonials as t}
			<div class="bg-white p-6 rounded-lg border border-gray-200 break-inside-avoid hover:border-brand-primary/30 transition-colors">
				<p class="font-mono text-xs leading-relaxed text-gray-700 mb-6">
					"{t.quote}"
				</p>
				<div class="flex items-center justify-between border-t border-gray-100 pt-4">
					<div class="flex items-center gap-3">
						<img src={t.image} alt={t.author} class="w-8 h-8 rounded-full bg-gray-200" />
						<div>
							<div class="text-xs font-bold text-gray-900">{t.author}</div>
							<div class="text-[10px] text-gray-500 font-mono">{t.role}</div>
						</div>
					</div>
                    <img src={t.icon} alt="Company Logo" class="w-5 h-5 rounded-sm opacity-70 grayscale" />
				</div>
			</div>
		{/each}
	</div>
</section>
