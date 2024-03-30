<script>
	let gopher = new URL('../lib/images/go-gopher.svg', import.meta.url).href;
	let react = new URL('../lib/images/react.png', import.meta.url).href;
	let jslogo = new URL('../lib/images/JS.png', import.meta.url).href;
	let python = new URL('../lib/images/python.png', import.meta.url).href;

	let desc = { hidden: false };
	function handleOpen() {
		desc = document.getElementById('proj-desc');
		desc.hidden = !desc.hidden;
	}
</script>

<div id="work-ex" class="p-4">
	<div class="bg-slate-50 border border-black p-4 rounded-lg">
		<div class="w-full flex justify-between">
			<p class="font-bold text-2xl">Projects</p>

			{#if desc.hidden}
				<button on:click={handleOpen} class="font-thin text-2xl">
					<svg
						xmlns="http://www.w3.org/2000/svg"
						fill="none"
						viewBox="0 0 24 24"
						stroke-width="1.5"
						stroke="currentColor"
						class="w-6 h-6"
					>
						<path stroke-linecap="round" stroke-linejoin="round" d="m19.5 8.25-7.5 7.5-7.5-7.5" />
					</svg>
				</button>
			{:else}
				<button on:click={handleOpen} class="font-thin text-2xl"
					><svg
						xmlns="http://www.w3.org/2000/svg"
						fill="none"
						viewBox="0 0 24 24"
						stroke-width="1.5"
						stroke="currentColor"
						class="w-6 h-6"
					>
						<path stroke-linecap="round" stroke-linejoin="round" d="m4.5 15.75 7.5-7.5 7.5 7.5" />
					</svg>
				</button>
			{/if}
		</div>
		<div id="proj-desc">
			<div class="flex items-center p-2">
				<img src={gopher} alt="bits-logo" class="border border-black h-12 w-12" />
				<div class="p-4">
					<p class="font-light text-xl">Blahblah: Chat Application</p>
					<p class="font-thin">A chat application built using Go, Templ, HTMX & TailwindCSS</p>
				</div>
			</div>
			<div class="flex items-center p-2">
				<img src={jslogo} alt="bits-logo" class="border border-black h-12 w-12" />
				<div class="p-4">
					<p class="font-light text-xl">JSEditor</p>
					<p class="font-thin">A rope based text editor built with JavaScript and Svelte</p>
				</div>
			</div>
			<div class="flex items-center p-2">
				<img src={react} alt="bits-logo" class="border border-black h-12 w-12" />
				<div class="p-4">
					<p class="font-light text-xl">Data Analyst Intern</p>
					<p class="font-thin">
						Uber, Hyderabad <span class="font-style: italic">(Jul 2023 - Present)</span>
					</p>
				</div>
			</div>
			<div class="flex items-center p-2">
				<img src={python} alt="bits-logo" class="border border-black h-12 w-12" />
				<div class="p-4">
					<p class="font-light text-xl">Software Development Intern</p>
					<p class="font-thin">
						VComply, Kolkata <span class="font-style: italic">(Jul 2023 - Present)</span>
					</p>
				</div>
			</div>
		</div>
	</div>
</div>
