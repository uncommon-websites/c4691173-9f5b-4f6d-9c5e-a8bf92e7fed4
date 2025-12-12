<script lang="ts">
	import { page } from "$app/state";
</script>

<main class="min-h-screen bg-white flex items-center justify-center px-4">
	<div class="text-center">
		<h1 class="text-8xl md:text-9xl font-thin tracking-tighter mb-4 uppercase">Error {page.status}</h1>
		<p class="text-sm uppercase tracking-wide mb-8 text-gray-500">{page.error?.message ?? "Something went wrong."}</p>
		<a href="/" class="inline-block bg-black text-white px-8 py-3 rounded-full text-[10px] font-bold uppercase tracking-widest hover:bg-gray-800 transition-colors">
			Go Back Home
		</a>
	</div>
</main>
