<script>
	let uber = new URL('../lib/images/uber_com_logo.jpeg', import.meta.url).href;
	let vcomply = new URL('../lib/images/vcomply_logo.jpeg', import.meta.url).href;
	function handleOpen() {
		const desc = document.getElementById('work-desc');
		desc.hidden = !desc.hidden;
	}
</script>

<div id="work-ex" class="p-4">
	<div class="border border-black rounded-lg p-4">
		<div class="w-full flex justify-between">
			<p class="font-bold text-2xl">Work Experience</p>
			<button on:click={handleOpen}>Open</button>
		</div>
		<div id="work-desc" hidden>
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
						VComply, Kolkata <span class="font-style: italic">(Jul 2023 - Present)</span>
					</p>
				</div>
			</div>
		</div>
	</div>
</div>
