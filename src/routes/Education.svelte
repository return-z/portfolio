<script>
	function handleOpen() {
		const desc = document.getElementById('edu-desc');
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
			<button on:click={handleOpen}>Open</button>
		</div>
		<div id="edu-desc" hidden>
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
