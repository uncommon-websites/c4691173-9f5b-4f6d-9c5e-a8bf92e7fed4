<script lang="ts">
	import Header from "$lib/components/Header.svelte";
	import { ArrowUpRight, ArrowRight } from 'lucide-svelte';

	const services = [
		{ id: '01', name: 'UX RESEARCH' },
		{ id: '02', name: 'USER INTERFACE DESIGN' },
		{ id: '03', name: 'PROTOTYPING' },
		{ id: '04', name: 'USER TESTING' },
		{ id: '05', name: 'DESIGN SYSTEMS' },
		{ id: '06', name: 'INTERACTION DESIGN' },
		{ id: '07', name: 'INFORMATION ARCHITECTURE' }
	];

	const projects = [
		{ name: 'HYBRID WORK TOOLS', category: 'PRODUCTIVITY APP', img: '/generated/image-designer-sketching-wireframes-on-paper-a-1765511708435-0.webp', description: 'Redesigning remote collaboration for distributed teams' },
		{ name: 'GAMING PLATFORM', category: 'ENTERTAINMENT', img: '/generated/image-close-up-of-hands-arranging-ui-design-ca-1765511712908-1.webp', description: 'Creating immersive user experiences for gamers' },
		{ name: 'AI DESIGN ASSISTANT', category: 'AI-POWERED TOOLS', img: '/generated/image-designer-reviewing-digital-prototypes-on-1765511716537-2.webp', description: 'Simplifying complex AI features for designers' },
		{ name: 'MOBILE BANKING', category: 'FINTECH', img: '/generated/image-young-designer-presenting-design-concept-1765511720011-3.webp', description: 'Building trust through intuitive financial interfaces' },
		{ name: 'HEALTH TRACKER', category: 'WELLNESS', img: '/generated/image-designer-working-on-laptop-with-design-s-1765511723443-4.webp', description: 'Motivating healthy habits through thoughtful design' },
		{ name: 'E-LEARNING PLATFORM', category: 'EDUCATION', img: '/generated/image-young-designer-working-focused-at-laptop-1765511741166-9.webp', description: 'Making online learning engaging and accessible' },
		{ name: 'SOCIAL COMMERCE', category: 'E-COMMERCE', img: '/generated/image-hands-sketching-user-flow-diagrams-in-no-1765511744694-10.webp', description: 'Bridging social media and shopping experiences' },
		{ name: 'SMART HOME APP', category: 'IOT', img: '/generated/image-designer-organizing-sticky-notes-on-wall-1765511748211-11.webp', description: 'Simplifying home automation for everyone' }
	];
</script>

<div class="min-h-screen bg-white text-[#1A1A1A] font-sans selection:bg-primary-500 selection:text-white overflow-x-hidden">
	<Header />

	<main>
		<!-- Hero Section -->
		<section class="pt-12 md:pt-20 pb-10 px-4 md:px-8" id="work">
			<div class="flex flex-col md:flex-row justify-between items-start mb-12 md:mb-24 relative">
				<div class="max-w-[200px] text-[10px] leading-relaxed uppercase tracking-wide font-medium mt-2">
					<p>Transforming complex UX challenges into intuitive digital experiences through research-driven design and prototyping.</p>
				</div>
				<h1 class="text-[14vw] md:text-[9rem] lg:text-[11rem] leading-[0.8] font-thin tracking-tighter text-right mt-8 md:mt-0 uppercase">
					Design <br />
					That
				</h1>
			</div>

			<!-- Hero Images -->
			<div class="grid grid-cols-5 gap-2 md:gap-4 mb-8 h-[30vh] md:h-[50vh]">
				<div class="overflow-hidden h-full bg-gray-100">
					<img src="/generated/image-designer-sketching-wireframes-on-paper-a-1765511708435-0.webp" alt="Designer sketching wireframes" class="w-full h-full object-cover hover:scale-110 transition-transform duration-1000" />
				</div>
				<div class="overflow-hidden h-full bg-gray-100">
					<img src="/generated/image-close-up-of-hands-arranging-ui-design-ca-1765511712908-1.webp" alt="UX research session" class="w-full h-full object-cover hover:scale-110 transition-transform duration-1000" />
				</div>
				<div class="overflow-hidden h-full bg-gray-100">
					<img src="/generated/image-designer-reviewing-digital-prototypes-on-1765511716537-2.webp" alt="Reviewing prototypes" class="w-full h-full object-cover hover:scale-110 transition-transform duration-1000" />
				</div>
				<div class="overflow-hidden h-full bg-gray-100">
					<img src="/generated/image-young-designer-presenting-design-concept-1765511720011-3.webp" alt="Design presentation" class="w-full h-full object-cover hover:scale-110 transition-transform duration-1000" />
				</div>
				<div class="overflow-hidden h-full bg-gray-100">
					<img src="/generated/image-designer-working-on-laptop-with-design-s-1765511723443-4.webp" alt="Designer at work" class="w-full h-full object-cover hover:scale-110 transition-transform duration-1000" />
				</div>
			</div>

			<div class="flex flex-col md:flex-row justify-between items-start">
				<span class="text-[10px] uppercase tracking-wide font-medium mt-4 hidden md:block">Scroll</span>
				<h1 class="text-[14vw] md:text-[9rem] lg:text-[11rem] leading-[0.8] font-thin tracking-tighter text-right w-full uppercase">
					Solves <br />
					Problems
				</h1>
			</div>
		</section>

		<!-- Services Section -->
		<section class="py-20 md:py-32" id="services">
			<div class="flex justify-center mb-16 md:mb-24">
				<span class="text-[10px] font-bold uppercase tracking-widest">Services</span>
			</div>

			<div class="border-t border-gray-200">
				{#each services as service}
					<div class="group border-b border-gray-200 py-6 md:py-10 px-4 md:px-8 flex items-center justify-between hover:bg-gray-50 transition-colors cursor-pointer">
						<span class="text-[10px] font-medium text-gray-400 w-8 md:w-12">/{service.id}</span>
						<h2 class="text-3xl md:text-6xl lg:text-7xl font-thin tracking-tight group-hover:italic transition-all duration-300 uppercase">{service.name}</h2>
						<div class="flex items-center gap-1 text-[10px] font-medium uppercase opacity-0 group-hover:opacity-100 transition-opacity translate-x-[-10px] group-hover:translate-x-0 duration-300">
							<ArrowUpRight size={12} />
							Learn More
						</div>
					</div>
				{/each}
			</div>
		</section>

		<!-- Projects Section -->
		<section class="py-20 px-4 md:px-8 bg-gray-50" id="projects">
			<div class="flex flex-col md:flex-row justify-between items-start mb-16 md:mb-24">
				<h2 class="text-4xl md:text-6xl font-light tracking-tight mb-8 md:mb-0 uppercase">Featured Projects</h2>
				<div class="max-w-xs text-[10px] leading-relaxed uppercase tracking-wide font-medium text-right md:text-left">
					<p>Portfolio-worthy case studies showcasing research-driven UX solutions for hybrid work tools, gaming platforms, and AI-powered design systems.</p>
				</div>
			</div>

			<div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-x-4 gap-y-12 md:gap-y-16">
				{#each projects as project}
					<div class="group cursor-pointer">
						<div class="aspect-[3/4] overflow-hidden mb-4 bg-gray-100">
							<img src={project.img} alt={project.name} class="w-full h-full object-cover group-hover:scale-105 transition-all duration-500" />
						</div>
						<h3 class="text-xs font-bold uppercase tracking-wide mb-1">{project.name}</h3>
						<p class="text-[10px] text-gray-500 uppercase tracking-wide mb-2">{project.category}</p>
						<p class="text-[10px] text-gray-600 leading-relaxed mb-3">{project.description}</p>
						<div class="inline-flex items-center gap-1 text-[10px] font-medium uppercase opacity-0 group-hover:opacity-100 transition-opacity">
							<ArrowUpRight size={10} />
							View Case Study
						</div>
					</div>
				{/each}
				
				<!-- More Projects Card -->
				<div class="flex flex-col justify-between h-full min-h-[300px] border border-gray-200 p-8 bg-white hover:bg-gray-50 transition-colors cursor-pointer group">
					<div class="flex justify-center items-center flex-1">
						<ArrowRight size={48} class="text-gray-200 group-hover:text-black transition-colors" />
					</div>
					<div>
						<h3 class="text-xs font-bold uppercase tracking-wide mb-1 leading-relaxed">Explore more<br/>design projects</h3>
						<div class="inline-flex items-center gap-1 text-[10px] font-medium uppercase mt-4">
							<ArrowUpRight size={10} />
							View All
						</div>
					</div>
				</div>
			</div>
		</section>

		<!-- About Section -->
		<section class="py-20 px-4 md:px-8" id="about">
			<div class="flex flex-col lg:flex-row mb-16 gap-12 lg:gap-24">
				<div class="flex-1">
					<h2 class="text-4xl md:text-6xl font-light tracking-tight uppercase">About Sebs Designs</h2>
				</div>
				<div class="flex-1">
					<h2 class="text-3xl md:text-5xl font-light tracking-tight mb-8 text-left uppercase leading-tight">Research-driven<br/>design solutions</h2>
					<div class="grid grid-cols-1 md:grid-cols-2 gap-8 text-[10px] leading-relaxed uppercase tracking-wide font-medium">
						<p>Sebs Designs specializes in transforming complex UX challenges into intuitive digital experiences. Through user research, iterative prototyping, and data-driven design decisions, we create solutions that users love.</p>
						<p>Our portfolio showcases real-world projects across hybrid work tools, gaming platforms, and AI-powered design systems. Each case study demonstrates systematic problem-solving, from initial research through final implementation, providing portfolio-worthy examples for aspiring designers.</p>
					</div>
					<a href="#contact" class="inline-flex items-center gap-1 text-[10px] font-medium uppercase mt-8 hover:opacity-60 transition-opacity">
						<ArrowUpRight size={10} />
						Get In Touch
					</a>
				</div>
			</div>

			<div class="flex flex-col md:flex-row gap-4 h-[50vh] md:h-[70vh]">
				<div class="w-full md:w-[60%] h-full bg-gray-100 overflow-hidden">
					<img src="/generated/image-modern-workspace-with-design-books-sketc-1765511726960-5.webp" alt="Design workspace" class="w-full h-full object-cover hover:scale-105 transition-transform duration-700" />
				</div>
				<div class="w-full md:w-[40%] h-full flex flex-col gap-4">
					<div class="flex-1 bg-gray-100 overflow-hidden">
						<img src="/generated/image-designer-conducting-user-testing-session-1765511730644-6.webp" alt="User testing session" class="w-full h-full object-cover hover:scale-105 transition-transform duration-700" />
					</div>
					<div class="flex-1 flex gap-4">
						<div class="flex-1 bg-gray-100 overflow-hidden">
							<img src="/generated/image-close-up-of-design-system-components-on--1765511734080-7.webp" alt="Design system" class="w-full h-full object-cover hover:scale-105 transition-transform duration-700" />
						</div>
						<div class="flex-1 bg-gray-100 overflow-hidden">
							<img src="/generated/image-designer-reviewing-mobile-app-prototypes-1765511737640-8.webp" alt="Mobile prototypes" class="w-full h-full object-cover hover:scale-105 transition-transform duration-700" />
						</div>
					</div>
				</div>
			</div>
		</section>

		<!-- CTA Section -->
		<section class="py-32 px-4 md:px-8 bg-gray-950 text-white text-center" id="contact">
			<span class="text-[10px] font-medium uppercase tracking-widest mb-6 block opacity-80">Build Your Portfolio</span>
			<h2 class="text-4xl md:text-6xl lg:text-8xl font-thin tracking-tight mb-12 uppercase">
				Ready to level up <br />
				your UX skills?
			</h2>
			<a href="mailto:hello@sebsdesigns.com" class="inline-block bg-primary-500 text-white px-10 py-4 rounded-full text-[10px] font-bold uppercase tracking-widest hover:bg-primary-600 transition-colors">
				Get In Touch
			</a>
		</section>

		<!-- Bottom Gallery -->
		<div class="grid grid-cols-2 md:grid-cols-5 h-[60vh]">
			<div class="overflow-hidden bg-gray-100">
				<img src="/generated/image-young-designer-working-focused-at-laptop-1765511741166-9.webp" alt="Designer at work" class="w-full h-full object-cover hover:scale-105 transition-transform duration-700" />
			</div>
			<div class="overflow-hidden bg-gray-100">
				<img src="/generated/image-hands-sketching-user-flow-diagrams-in-no-1765511744694-10.webp" alt="Sketching user flows" class="w-full h-full object-cover hover:scale-105 transition-transform duration-700" />
			</div>
			<div class="overflow-hidden bg-gray-100">
				<img src="/generated/image-designer-organizing-sticky-notes-on-wall-1765511748211-11.webp" alt="Ideation session" class="w-full h-full object-cover hover:scale-105 transition-transform duration-700" />
			</div>
			<div class="overflow-hidden bg-gray-100">
				<img src="/generated/image-close-up-of-designers-hands-using-stylus-1765511751808-12.webp" alt="Digital design work" class="w-full h-full object-cover hover:scale-105 transition-transform duration-700" />
			</div>
			<div class="overflow-hidden hidden md:block bg-gray-100">
				<img src="/generated/image-designer-reviewing-design-feedback-durin-1765511755322-13.webp" alt="Design collaboration" class="w-full h-full object-cover hover:scale-105 transition-transform duration-700" />
			</div>
		</div>

		<!-- Footer Marquee -->
		<div class="overflow-hidden py-6 border-b border-gray-200">
			<div class="whitespace-nowrap animate-marquee flex">
				<span class="text-4xl md:text-6xl lg:text-8xl font-thin tracking-tight mx-4 uppercase">Design that solves problems — Design that solves problems — Design that solves problems — </span>
				<span class="text-4xl md:text-6xl lg:text-8xl font-thin tracking-tight mx-4 uppercase">Design that solves problems — Design that solves problems — Design that solves problems — </span>
			</div>
		</div>
	</main>

	<footer class="px-4 md:px-8 py-12 text-[10px] font-medium uppercase tracking-wide">
		<div class="flex flex-col md:flex-row justify-between items-start md:items-end gap-12 md:gap-8">
			<div class="flex flex-col gap-3">
				<a href="#work" class="hover:opacity-60">Work</a>
				<a href="#services" class="hover:opacity-60">Services</a>
				<a href="#projects" class="hover:opacity-60">Projects</a>
				<a href="#about" class="hover:opacity-60">About</a>
			</div>

			<div class="text-left md:text-center">
				<p class="text-lg md:text-2xl font-normal tracking-tight mb-6">HELLO@SEBSDESIGNS.COM</p>
				<p class="text-xs tracking-widest text-gray-500">PORTFOLIO-WORTHY UX PROJECTS</p>
			</div>

			<div class="flex flex-col gap-3 text-left md:text-right">
				<a href="https://www.behance.net" target="_blank" rel="noopener noreferrer" class="hover:opacity-60">Behance</a>
				<a href="https://dribbble.com" target="_blank" rel="noopener noreferrer" class="hover:opacity-60">Dribbble</a>
			</div>
		</div>

		<div class="flex flex-col md:flex-row justify-between items-center mt-20 pt-8 border-t border-gray-200 text-[10px] text-gray-400 gap-4">
			<p>© 2024 SEBS DESIGNS. ALL RIGHTS RESERVED</p>
			<div class="flex items-center gap-2">
				<svg class="w-5 h-5 text-black" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
					<rect x="4" y="4" width="11" height="11" rx="2" fill="currentColor" />
					<rect x="9" y="9.5" width="10" height="10" rx="2" fill="currentColor" fill-opacity="0.24" />
				</svg>
				<span class="text-black text-lg font-bold tracking-tight">SEBS DESIGNS</span>
			</div>
			<p>UX/UI DESIGN PORTFOLIO</p>
		</div>
	</footer>
</div>

<style>
	@keyframes marquee {
		0% { transform: translateX(0); }
		100% { transform: translateX(-50%); }
	}
	.animate-marquee {
		animation: marquee 30s linear infinite;
	}
</style>

