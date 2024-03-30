<script>
	let desc = { hidden: false };
	function handleOpen() {
		desc = document.getElementById('edu-desc');
		desc.hidden = !desc.hidden;
	}
	let src = new URL(
		'../lib/images/birla_institute_of_technology_and_science_pilani_logo.jpeg',
		import.meta.url
	).href;
</script>

<div id="education" class="p-4">
	<div class="border border-black rounded-lg p-4 bg-slate-50">
		<div class="flex justify-between">
			<p class="font-bold text-2xl">Education</p>

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
		<div id="edu-desc">
			<div class="flex items-center p-2">
				<img {src} alt="bits-logo" class="border border-black h-12 w-12" />
				<div class="p-4">
					<p class="font-light text-xl">Birla Institute of Technology & Science, Pilani</p>
					<p class="font-thin">
						B.E.(Hons.) Electrical & Electronics Engineering <span class="font-style: italic"
							>(2019-2024)</span
						>
					</p>
				</div>
			</div>
		</div>
	</div>
</div>
