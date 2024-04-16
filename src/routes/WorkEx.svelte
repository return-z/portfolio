<script>
	let uber = new URL('../lib/images/uber_com_logo.jpeg', import.meta.url).href;
	let vcomply = new URL('../lib/images/vcomply_logo.jpeg', import.meta.url).href;
	let desc = { hidden: false };
	function handleOpen() {
		desc = document.getElementById('work-desc');
		desc.hidden = !desc.hidden;
	}
</script>

<div id="work-ex" class="p-4">
	<div class="bg-slate-50 border border-black rounded-lg p-4">
		<div class="w-full flex justify-between">
			<p class="font-bold text-2xl">Work Experience</p>
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
		<div id="work-desc">
			<div class="flex items-center p-2">
				<img src={uber} alt="bits-logo" class="border border-black h-12 w-12" />
				<div class="p-4">
					<p class="font-light text-xl">Data Analyst Intern</p>
					<p class="font-thin">
						Uber, Hyderabad <span class="font-style: italic">(Jul 2023 - Present)</span>
					</p>
				</div>
			</div>
			<div class="flex items-center p-2">
				<img src={vcomply} alt="bits-logo" class="border border-black h-12 w-12" />
				<div class="p-4">
					<p class="font-light text-xl">Software Development Intern</p>
					<p class="font-thin">
						VComply, Kolkata <span class="font-style: italic">(May 2021 - Jul 2021)</span>
					</p>
				</div>
			</div>
		</div>
	</div>
</div>
