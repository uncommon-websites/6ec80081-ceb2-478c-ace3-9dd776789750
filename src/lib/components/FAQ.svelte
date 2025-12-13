<script lang="ts">
	import { slide } from 'svelte/transition';

	const faqs = [
		{
			question: "Is Avalonia UI really free?",
			answer: "Yes! Avalonia UI is completely free and open source under the MIT license. You can use it in any project, commercial or personal, without any fees or restrictions."
		},
		{
			question: "What platforms does Avalonia UI support?",
			answer: "Avalonia UI supports Windows, macOS, Linux, iOS, Android, and WebAssembly. You write your code once and deploy it to all platforms."
		},
		{
			question: "How is Avalonia UI different from MAUI or Uno Platform?",
			answer: "Avalonia UI focuses on desktop-first development with exceptional performance and a mature XAML implementation. It has been production-ready for years and powers thousands of applications worldwide."
		},
		{
			question: "Can I use my existing WPF or UWP knowledge?",
			answer: "Absolutely! Avalonia UI uses XAML syntax very similar to WPF and UWP. Most WPF developers can start building with Avalonia UI immediately with minimal learning curve."
		},
		{
			question: "What IDEs and tools are supported?",
			answer: "Avalonia UI works with Visual Studio, Visual Studio Code, and JetBrains Rider. We provide extensions for IntelliSense, XAML preview, and hot reload support."
		},
		{
			question: "How is the performance compared to native apps?",
			answer: "Avalonia UI uses hardware-accelerated rendering and compiles to native code, delivering performance comparable to native applications on each platform."
		},
		{
			question: "Where can I get help and support?",
			answer: "Join our active community on GitHub Discussions, Discord, and Telegram. We also have comprehensive documentation, tutorials, and sample applications to help you get started."
		}
	];

	let openIndex: number | null = null;

	function toggle(index: number) {
		openIndex = openIndex === index ? null : index;
	}
</script>

<section class="py-24 px-6 md:px-12 max-w-7xl mx-auto border-t border-gray-200">
	<div class="grid grid-cols-1 lg:grid-cols-3 gap-12">
		<div>
			<span class="font-mono text-[10px] text-gray-500 uppercase tracking-widest mb-4 block">
				[ FAQ ]
			</span>
			<h2 class="font-display text-4xl md:text-5xl font-medium tracking-tight text-gray-900 mb-6">
				Frequently Asked Questions
			</h2>
			<p class="font-mono text-sm text-gray-600 mb-8">
				Your question not answered here?
			</p>
			<button class="bg-brand-green text-white px-5 py-2.5 rounded text-sm font-medium hover:bg-brand-green-hover transition-colors flex items-center gap-2 font-mono uppercase tracking-wide text-xs">
				<svg xmlns="http://www.w3.org/2000/svg" width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M21 15a2 2 0 0 1-2 2H7l-4 4V5a2 2 0 0 1 2-2h14a2 2 0 0 1 2 2z"/></svg>
				Contact Us
			</button>
		</div>

		<div class="lg:col-span-2 space-y-4">
			{#each faqs as faq, i}
				<div class="border-b border-gray-200 pb-4">
					<button class="w-full flex items-center justify-between text-left py-2 group" on:click={() => toggle(i)}>
						<span class="font-mono text-sm font-medium text-gray-800 group-hover:text-brand-primary transition-colors pr-8">{faq.question}</span>
						<svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="text-gray-400 transition-transform duration-300 {openIndex === i ? 'rotate-180' : ''}"><path d="m6 9 6 6 6-6"/></svg>
					</button>
					{#if openIndex === i}
						<div transition:slide={{ duration: 300 }} class="overflow-hidden">
							<p class="pt-2 pb-4 text-sm text-gray-600 leading-relaxed max-w-2xl font-mono">
								{faq.answer}
							</p>
						</div>
					{/if}
				</div>
			{/each}
		</div>
	</div>
</section>
