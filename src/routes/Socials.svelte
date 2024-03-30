<script>
	let dp = new URL('../lib/images/profile_pic.jpeg', import.meta.url).href;
	let git = new URL('../lib/images/github.png', import.meta.url).href;
	let linkedin = new URL('../lib/images/linkedin.png', import.meta.url).href;
</script>

<div id="info" class="flex justify-center flex-col">
	<div class="flex justify-center w-full">
		<img src={dp} alt="pic" class="overflow-hidden h-20 w-20 rounded-full" />
	</div>
	<p class="p-2 text-2xl justify-center font-bold">Vinayak Tyagi</p>
	<div class="flex flex-row items-center justify-center">
		<img src={git} alt="git" class="w-6 h-6" />
		<p class="p-2 text-xl font-thin">GitHub</p>
	</div>
	<div class="flex flex-row items-center justify-center">
		<img src={linkedin} alt="git" class="w-6 h-6" />
		<p class="p-2 text-xl font-thin">LinkedIn</p>
	</div>
</div>
