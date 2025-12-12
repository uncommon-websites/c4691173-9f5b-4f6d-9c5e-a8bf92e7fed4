<script lang="ts">
	import { ArrowUpRight } from 'lucide-svelte';
</script>

<header class="w-full px-4 md:px-8 py-6 flex items-center justify-between text-[10px] font-medium tracking-wide uppercase border-b border-transparent fixed top-0 left-0 z-50 bg-white/90 backdrop-blur-sm transition-all duration-300">
	<div class="flex-1">
		<a href="/" class="flex items-center gap-2">
			<svg class="w-6 h-6 text-black" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
				<rect x="4" y="4" width="11" height="11" rx="2" fill="currentColor" />
				<rect x="9" y="9.5" width="10" height="10" rx="2" fill="currentColor" fill-opacity="0.24" />
			</svg>
			<span class="text-xl font-medium tracking-tighter">SEBS DESIGNS</span>
		</a>
	</div>

	<nav class="hidden md:flex items-center gap-12 text-gray-500">
		<a href="#work" class="hover:text-black transition-colors">Work</a>
		<a href="#services" class="hover:text-black transition-colors">Services</a>
		<a href="#projects" class="hover:text-black transition-colors">Projects</a>
		<a href="#about" class="hover:text-black transition-colors">About</a>
	</nav>

	<div class="flex-1 flex justify-end items-center gap-6 md:gap-8">
		<a href="#contact" class="flex items-center gap-1 hover:opacity-70 transition-opacity">
			<ArrowUpRight size={14} />
			GET IN TOUCH
		</a>
	</div>
</header>
