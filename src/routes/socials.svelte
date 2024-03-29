<script>
	let src = new URL('../lib/images/profile_pic.jpeg', import.meta.url).href;
</script>

<div id="info" class="flex flex-col">
	<div class="flex justify-center w-full">
		<img {src} alt="pic" class="flex rounded-lg object-contain h-20 w-20" />
	</div>
	<p class="p-2 text-2xl font-bold">Vinayak Tyagi</p>
	<p class="p-2 text-xl font-thin">GitHub</p>
	<p class="p-2 text-xl font-thin">LinkedIn</p>
	<p class="p-2 text-xl font-thin">Instagram</p>
</div>
